# LightOpenId

This is a modified version of [LightOpenId by mewp on Gitorious](https://gitorious.org/lightopenid). It allows client to force a specific OpenId endpoint URL. This is useful for organization applications wishing to authenticate with Google Apps Federated Login. You can specify the Google Apps Federated Login endpoint url directly with:

    $openid = new LightOpenId('localhost'); // replace with your host
    $openid->version = 2;
    $openid->server = 'https://www.google.com/a/YOURDOMAIN.com/o8/ud?be=o8';
    $openid->identity = 'http://specs.openid.net/auth/2.0/identifier_select';
    
For more usage examples, see `example.php` and `example-google.php`.