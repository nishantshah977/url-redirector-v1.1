<?php
$url=$_POST['url'];
$link=$_POST['link'];
if(file_exists($link)){
    echo "Sorry Select Another Link";
    return 0;
}
$file = fopen($link,"a");
fwrite($file,'<html><head><link rel="stylesheet" href="/style.css"/>
<meta name="viewport" content="width=device-width, initial-scale=1.0"><META NAME="robots" CONTENT="noindex,nofollow">
</head>
<body>');
fwrite($file,'<script> var redirect ="'.$url.'";');
$hi =file_get_contents("function.txt");
$fi = file_get_contents($link);
if ($hi !== $fi){
    file_put_contents($link, $hi,FILE_APPEND);
    echo 'Success Please <a href="https://geekhelper.000webhostapp.com/'.$link.'">Click Here</a>';
}
    ?>







