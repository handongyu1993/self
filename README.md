# MBTI图片资源服务

这是一个用于托管MBTI相关图片的静态资源服务。

## 目录结构

- `/cloud_images/` - MBTI相关图片资源
  - 16种MBTI类型图片 (如 `istj.png`, `enfp.png` 等)
  - `mbti-logo.png` - MBTI标志图片

## 使用方法

图片资源可通过以下URL格式访问：

```
https://您的域名/cloud_images/图片名称.png
```

例如：
```
https://您的域名/cloud_images/istj.png
https://您的域名/cloud_images/mbti-logo.png
```

## 部署方式

该项目使用Vercel进行部署，通过以下配置实现静态资源服务：

- `vercel.json` - 配置静态资源路由和缓存策略
- `index.html` - 提供简单的资源目录页面

## 常见问题

### 无法访问图片

如果无法访问图片，请检查：

1. 图片URL是否正确
2. 图片文件名是否区分大小写（应全部小写）
3. vercel.json配置是否正确
4. 是否有跨域访问限制 