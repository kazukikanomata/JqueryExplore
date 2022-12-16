# JqueryExplore
htmlとCSSが読み込まれた後にJqueryが読み込まれる。

## セレクタ →　何を
$("p");

## メソッド　→　どうする
.css("color", "red");

## イベント
<p>click mousehover change</p>;

## animate
### キャメルケースで書くこと
$("セレクタ").animate({
    "プロパティ": "値",
    "プロパティ": "値",
    "プロパティ": "値"
});

### duraiton
$("セレクタ").animate({
    "プロパティ": "値",
    "プロパティ": "値",
    "プロパティ": "値"
},
{
    duration:3000
});
### 関数の書式
$(function(){
    function 関数名(){
        処理内容
    }
});

### 例
$(function(){
    function color_width (){
        $(this).css("color", "#ccc");
        $(this).css("width", "300px");			
    }
    $(".box1").on("mouseover", color_width);
    $(".box2").on("mouseover", color_width);
    $(".box3").on("mouseover", color_width);
});
