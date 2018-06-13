# Curl - PHP
Advanced Curl Library

#### Curl::post
```php
// You can register a variable, or initiate a callback.
$curl = Curl::post(

  // Setup url and fields
  array(
    'url' => 'http://example.com',
    'fields' => array(
      'data' => 'password'
    )
  ),
  
  // Setup additional curl options
  array (
      CURLOPT_URL => 'https://example.com'
  )
  
  /*
  ,
  // Callback function after executed, returns response and curl info
  function($response, $info) {
    print_r($response);
  }
  */
);

// get response
print_r($curl->response);

// get info
print_r($curl->info);

```
#### Curl::get

```php
Curl::get(

  // Setup url and fields
  array(
    'url' => 'http://example.com',
    'fields' => array(
      'data' => 'password'
    )
  ),
  
  // Setup additional curl options
  array (
      CURLOPT_URL => 'https://example.com'
  ),
  
  // Callback function after executed, returns response and curl info
  function($response, $info) {
    print_r($response);
  }

);
```
