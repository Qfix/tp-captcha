# think-captcha

thinkphp6 验证码类库

## 安装
> composer require fixed/tp-captcha



## 使用

~~~
 $captcha = new Captcha();
  $captcha->create();
~~~

## 验证

~~~
 $captcha = new Captcha();
$uniqid = 'cbf196301a389c284552f4379a4a159b';
$code = 'vdmn';
if ($captcha->check($uniqid, $code) === true) {
    echo 1;
} else {
    echo 0;
}
~~~

