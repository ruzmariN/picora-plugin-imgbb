# ImgBB 图床

通过 [ImgBB API](https://api.imgbb.com/) 为 Picora 添加图片上传支持。上传成功后使用 API 返回的图片直链，并读取缩略图链接。

## 使用方法

1. 前往 [ImgBB API 页面](https://api.imgbb.com/) 获取 API Key。
2. 在 Picora 1.0.1 或更新版本中导入本插件的 ZIP。
3. 新建「ImgBB 图床」配置，填入 API Key，选择图片上传。

插件只向 `https://api.imgbb.com/1/upload` 发送 POST 请求，请求体为 multipart/form-data，图片字段为 `image`。API Key 作为 `key` 查询参数传递；请妥善保管，勿公开包含它的请求地址。插件不会跟随重定向，也不会自动重传上传请求。

## 图床说明
1. ImgBB图床的最大上传限制为32mb
2. Picora目前不支持图像删除，如果你想删除已上传的图片请到ImgBB登录你的账户手动删除。
3. 请勿上传违反图床使用条款或违反当地法律的图片。

## 许可

[MIT](LICENSE)。
> 这是第三方适配插件，不代表 ImgBB 官方。

