<?php
$secret = "0x4AAAAAABkNY4DJYu1LiA7xR-ueRhXaugzGM";
$token = $_POST['cf-turnstile-response'];

$url = "https://challenges.cloudflare.com/turnstile/v0/siteverify";
$data = [
    'secret' => $secret,
    'response' => $token
];

$options = [
    'http' => [
        'header'  => "Content-type: application/x-www-form-urlencoded\r\n",
        'method'  => 'POST',
        'content' => http_build_query($data)
    ]
];

$context = stream_context_create($options);
$result = file_get_contents($url, false, $context);
$response = json_decode($result);

if (!$response->success) {
    die("人机验证失败！错误代码: " . implode(", ", $response->{"error-codes"}));
}

// 验证通过，继续处理表单
?>
