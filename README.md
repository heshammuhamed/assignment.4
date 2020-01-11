<?php

function calcArray($array){
    
$sum=0;
foreach ($array as $item){
    $sum=$sum+$item;
}
echo $sum;

}$arr1=array(5,8,9,3,6);
calcArray($arr1);
echo "<hr/>";


function Languages($arrLanguages) {
foreach($arrLanguages as $language) {
echo $language . " - ";
}
}
$languages = array('php','paython','wordpress');
Languages($languages);

echo "<hr/>";


function RouteBinarySearch( $arr, $i) {
    if (count($arr) === 0) return false; 
     $low = 0; 
    $high = count($arr) - 1; 
     while ($low <= $high) { 
      $mid = floor(($low + $high) / 2); 
       if($arr[$mid] == $i) { 
            return true; 
        } 
  
        if ($i < $arr[$mid]) { 
            $high = $mid -1; 
        } 
        else { 
            $low = $mid + 1; 
        } 
    } 
    return false; 
} 
$arr = array(1, 2, 3, 4, 5); 
$value = 5; 
if(RouteBinarySearch($arr, $value) == true) { 
    echo "Yes";
} 
else { 
    echo "No";
} 
echo "<hr/>";

$n=7; 
function getName($n) { 
    $characters = 'heshammohamed'; 
    $randomString = ''; 
  
    for ($i = 0; $i < $n; $i++) { 
        $index = rand(0, strlen($characters) - 1); 
        $randomString .= $characters[$index]; 
    } 
  
    return $randomString; 
} 
  
echo getName($n); 

