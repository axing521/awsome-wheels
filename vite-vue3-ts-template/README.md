# vite-vue3-ts的工程模板

您可以将您的项目作为一个模板存储在本地或者远程仓库中，然后使用vite的模板创建命令来创建新的项目。具体操作步骤如下：

1. 在您的项目根目录下创建一个`template.json`文件，用于描述您的模板信息，例如模板名称、版本号、作者等。

2. 在您的项目根目录下执行以下命令，将您的项目作为vite的模板注册到本地模板列表中：

   ```
   vite add template <template-name> ./
   ```

   其中，`<template-name>`为您的模板名称，`.`表示当前目录。

3. 现在您可以使用以下命令来创建新的项目：

   ```
   vite create <project-name> --template <template-name>
   ```

   其中，`<project-name>`为您要创建的项目名称，`<template-name>`为您的模板名称。

   这样，vite就会使用您的模板来创建新的项目了。

template.json样例

```json
{
  "name": "my-template",
  "version": "1.0.0",
  "description": "My Vite template",
  "author": "John Doe",
  "repository": {
    "type": "git",
    "url": "https://github.com/johndoe/my-template.git"
  },
  "keywords": [
    "vite",
    "template"
  ],
  "dependencies": {
    "vue": "^3.0.0"
  },
  "devDependencies": {
    "@vitejs/plugin-vue": "^1.0.0"
  }
}
```

