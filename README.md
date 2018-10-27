<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
<html xmlns="http://www.w3.org/1999/xhtml">
<head>
<meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
<title>快速排序</title>
</head>

<body>
#快速排序<br />
&quot;&quot;&quot;<br />
def quicksort(array):<br />
if len(array) &lt; 2:<br />
return array<br />
else:<br />
pivot = array[0]<br />
less = [i for i in array[1:] if i &lt;=pivot]<br />
greater = [i for i in array[1:] if i &gt;pivot]<br />
return quicksort(less) + [pivot] + quicksort(greater)<br />
arr = [6,45,68,15,34,56,78,5,94,646,642,54,8,78,54,64,315,354,46,89,97]<br />
print (quicksort(arr)) <br />
&quot;&quot;&quot;<br />
def quicksort(array):<br />
if len(array) &lt; 2:<br />
return array<br />
else:<br />
less = []<br />
greater = []<br />
pivot = array[0]<br />
for i in array[1:]:<br />
if i &lt;= pivot:<br />
less.append(i)<br />
else:<br />
greater.append(i)<br />
return quicksort(less) + [pivot] + quicksort(greater)<br />
arr = [6,45,68,15,34,56,78,5,94,646,642,54,8,78,54,64,315,354,46,89,97]<br />
print(quicksort(arr))
</body>
</html>
