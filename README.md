# RAGFlow_MinIO_images

原因：RAGFlow作为外部知识库，不支持处理图片链接服务\n

解决方法：RAGFlow知识库预处理文档支持markdown格式图片链接，再上传知识库。即可使用nginx反代访问图片\n

## 操作示例
1、拉取项目，确认结构\n
![1](doc/images/1.png)\n
2、修改为你RAGFlow的对象存储MinIO的地址、密码、存储图片的桶\n
![6](doc/images/6.png)\n
3、把要处理的文档放到input_documents文件夹\n
![2](doc/images/2.png)\n
4、安装python依赖包，执行py脚本，查看日志\n
![3](doc/images/3.png)\n
5、登录MinIO查看桶上传的图片\n
![4](doc/images/4.png)\n
6、到output_documents查看处理好的文档\n
![5](doc/images/5.png)\n
7、使用nginx反代访问图片\n
8、更多。修改脚本的保存图片链接，加上地址可以直接访问\n
