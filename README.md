# 用户中心前端

最大的坑点在于: 
1.Docker部署上线时,从github上拉取的前端代码,没有dist目录,如果不手动上传构建好的dist文件夹,DockerFile是找不到的,一定要记住这一点!!!
2. dockerFile 的FROM nginx 记得带上nginx版本 如 : FROM nginx:1.18

## Environment Prepare

Install `node_modules`:

```bash
npm install
```

or

```bash
yarn
```

## Provided Scripts

鱼皮用户中心 provides some useful script to help you quick start and build with web project, code style check and test.

Scripts provided in `package.json`. It's safe to modify or add additional script:

### Start project

```bash
npm start
```

### Build project

```bash
npm run build
```

### Check code style

```bash
npm run lint
```

You can also use script to auto fix some lint error:

```bash
npm run lint:fix
```

### Test code

```bash
npm test
```

## More

You can view full document on our [official website](https://pro.ant.design). And welcome any feedback in our [github](https://github.com/ant-design/ant-design-pro).
