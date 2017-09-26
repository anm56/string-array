<?php
$array= array(1,2,3,4,5,6,7);
class main
{
  public function printarray($array)
  {
  echo '<h1>print array demo</h1>';
  print_r($array);
  echo '<hr>';
 }
 public function uppercase()
  {
   echo '<h1>uppercase array demo </h1>';
   $array1=array("hello"=>"5","world"=>"5");
   print_r(array_change_key_case($array1,CASE_UPPER));
    echo '<hr>';
  }
public function arraychunk()
    {
   echo '<h1> array chunk demo</h1>';
   $array2=array(a,b,c,d,e,f);
    print_r(array_chunk($array2,2));
     echo '<hr>';
    }
public function arrcombine()
    {
     echo '<h1>array combine demo</h1>';
     $array3=array(A,B,C);
     $array4=array(Apple,Banana,Chickoo);
     $array5=array_combine($array3,$array4);
     print_r($array5);
     echo '<hr>';
   }
 public function arrcount()
     {
    echo '<h1>array count demo</h1>';
    $array6=array(Cat,Dog,Cat,Dog,monkey);
    print_r(array_count_values($array6));
    echo '<hr>';
     }
 public function arrmerge()
         {
	 echo '<h1> array merge demo</h1>';
	 $array7=array("Have","a");
	 $array8=array("great","day");
	 $result=array_merge($array7,$array8);
	 print_r($result);
	 echo '<hr>';
	 }
 public function arrsort()
	  {
	  echo '<h1> array sort demo</h1>';
          $array9=array(20,70,30,90);
	  $array10=array(7,3,5,9);
	   array_multisort($array9,$array10);
	   var_dump($array9);
	   var_dump($array10);
	    echo '<hr>';
	   }
public function arrproduct()
	   {
	   echo '<h1>array product demo</h1>';
	   $array11=array(2,3,4,5);
	   echo array_product($array11);
	   echo '<hr>';
	   }
public function arrreverse()
	   {
	   echo '<h1> array reverse demo</h1>';
           $input=array(1,2,3,4,5);
	   $reverse=array_reverse($input);
	     print_r($input);
	     print_r($reverse);
	    echo '<hr>';
            }
public function arrsearch()
	    {
            echo '<h1>array search demo</h1>';
	    $array12=array(0=>'red',1=>'blue',2=>'yellow');
	    $search=array_search('blue',$array12);
            print_r($array12);
	    echo"<br/>";
	    echo "$search";
	    echo '<hr>';
	    }
       	}
	$obj=new main();
	$obj->printarray($array);
	$obj->uppercase();
	$obj->arraychunk();
	$obj->arrcombine();
	$obj->arrcount();
	$obj->arrmerge();
	$obj->arrsort();
	$obj->arrproduct();
	$obj->arrreverse();
	$obj->arrsearch();
	?>
