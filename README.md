## PHP Javascript UnPacker

```
$source = "eval(function(p,a,c,k,e,r){e=String;if(!''.replace(/^/,String)){while(c--)r[c]=k[c]||c;k=[function(e){return r[e]}];e=function(){return'\\w+'};c=1};while(c--)if(k[c])p=p.replace(new RegExp('\\b'+e(c)+'\\b','g'),k[c]);return p}('0.1(\'2 3\');',4,4,'console|log|hello|world'.split('|'),0,{}))";

$unpacker = new JavascriptUnpacker;

echo $unpacker->unpack($source);  // console.log('hello world');
```

Packagist: https://packagist.org/packages/duyplus/php-javascript-unpacker
