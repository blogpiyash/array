# array
array_merge_recursive()
```
- Used to Merge one or more arrays into single array recursively.
```
Example:
```
<?php


$a1 = [
    'value1' => 'piyash',
    'value2' => '33'
];

$a2 = [
    'value1' => 'ahasan'
];

$result = array_merge_recursive($a1, $a2);
print_r($result);


?>
```
```
result:
===

 Array
(
    [value1] => Array
        (
            [0] => piyash
            [1] => ahasan
        )

    [value2] => 33
)
 ```
 
array_merge()
```
- used to merge two or more arrays into a single array. 
- But, If two elements have the same string keys(value1) then the latter value will be overridden.
```

Example:
```
<?php


$a1 = [
    'value1' => 'piyash',
    'value2' => '33'
];

$a2 = [
    'value1' => 'ahasan'
];

$result = array_merge($a1, $a2);
print_r($result);


?>
```
```
result:
===

Array
(
    [value1] => ahasan
    [value2] => 33
)
 ```
