---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php

// THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphServiceClient = new GraphServiceClient($requestAdapter);

$requestBody = new PhoneAuthenticationMethod();
$requestBody->setPhoneNumber('+1 2065555554');

$requestBody->setPhoneType(new AuthenticationPhoneType('mobile'));



$result = $graphServiceClient->me()->authentication()->phoneMethodsById('phoneAuthenticationMethod-id')->patch($requestBody);


```