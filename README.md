# qcloud_cos_p3

fork from [https://github.com/a270443177/cos-python3-sdk-v4](https://github.com/a270443177/cos-python3-sdk-v4)

fix bug and make it simple to use


~~~
from qcloud_cos.cos_cred import CredInfo
from qcloud_cos.cos_auth import Auth

cred = CredInfo(appId, u'secretId', u'secretKey')
auth_obj = Auth(cred)
sign_str = auth_obj.sign_more(u'bucket', u'/cos_path/', int(time.time()) + 60)
~~~