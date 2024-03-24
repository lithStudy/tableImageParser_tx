# tableImageParser

### 本项目通过腾讯分享文章，复现了腾讯表格结果解析文章地址为https://zhuanlan.zhihu.com/p/69793742   (Table Structure Recognition from Tencent)

## 环境(Requirements)
```pip install -r requirements.txt```

## 例子🌰(Demo)
- 修改inference 中main函数所需路径

```python inference.py```

## 训练(train)
- 修改train.py 中checkpoint_path 为模型路径
- 修改dataf.py 中training_data_path 为训练数据路径

```python train.py```

## 可视化实例
### 例子🌰1
![raw](https://github.com/tommyMessi/tableImageParser_tx/blob/master/tx_infer_data/vanke_2016_1241_nb_3.jpg)
![nrow](https://github.com/tommyMessi/tableImageParser_tx/blob/master/tx_infer_data/nrow/vanke_2016_1241_nb_3.jpg)
![ncol](https://github.com/tommyMessi/tableImageParser_tx/blob/master/tx_infer_data/ncol/vanke_2016_1241_nb_3.jpg)
### 例子🌰2
![raw](https://github.com/tommyMessi/tableImageParser_tx/blob/master/tx_infer_data/1.jpg)
![row](https://github.com/tommyMessi/tableImageParser_tx/blob/master/tx_infer_data/row/1.jpg)
![row](https://github.com/tommyMessi/tableImageParser_tx/tree/master/tx_infer_data/col)

## 更新 8.17
- 修改dataf.py 中的数据预处理，具体效果 根据自己数据进行适量修改。（数据增强对效果还很重要）
- 添加post.py 用于后处理的demo。具体思路通过霍夫变换的HoughLinesP函数的线段合集，进行直线断连接修复。
- 预训练模型： 链接: https://pan.baidu.com/s/1JXEKuWYtbyF6vFGQIzyE6g 提取码: 4mbb

## 其他
训练数据与预训练模型 关注微信公众账号 hulugeAI 留言：table parser



## 我的试用补充
模型地址：
链接：https://pan.baidu.com/s/1n6t2TSoZ1cIJhYXjd_R9dg?pwd=zogb

数据集作者目前已经不开放了

对于扫描出来的有线和无线表格的行列分析效果都还不错，手拍的效果比较差，但是个人感觉这个项目本身的思路没有问题，如果有更多的数据集可能效果会比较好

这个项目用工具集的版本比较老，安装会有一些问题，因此我使用的新的版本安装的，有一些适配问题，需要改一些代码



| Name                      | Version    | Build              | Channel       |
|---------------------------|------------|--------------------|---------------|
| absl-py                   | 2.1.0      | pypi_0             | pypi          |
| asttokens                 | 2.4.1      | pypi_0             | pypi          |
| astunparse                | 1.6.3      | pypi_0             | pypi          |
| backcall                  | 0.2.0      | pypi_0             | pypi          |
| ca-certificates           | 2024.3.11  | haa95532_0         |               |
| cachetools                | 5.3.3      | pypi_0             | pypi          |
| certifi                   | 2024.2.2   | pypi_0             | pypi          |
| charset-normalizer        | 3.3.2      | pypi_0             | pypi          |
| colorama                  | 0.4.6      | pypi_0             | pypi          |
| contourpy                 | 1.1.1      | pypi_0             | pypi          |
| cycler                    | 0.12.1     | pypi_0             | pypi          |
| decorator                 | 5.1.1      | pypi_0             | pypi          |
| executing                 | 2.0.1      | pypi_0             | pypi          |
| flask                     | 0.10.1     | pypi_0             | pypi          |
| flatbuffers               | 24.3.7     | pypi_0             | pypi          |
| fonttools                 | 4.50.0     | pypi_0             | pypi          |
| gast                      | 0.4.0      | pypi_0             | pypi          |
| google-auth               | 2.29.0     | pypi_0             | pypi          |
| google-auth-oauthlib      | 0.4.6      | pypi_0             | pypi          |
| google-pasta              | 0.2.0      | pypi_0             | pypi          |
| grpcio                    | 1.62.1     | pypi_0             | pypi          |
| h5py                      | 3.10.0     | pypi_0             | pypi          |
| idna                      | 3.6        | pypi_0             | pypi          |
| importlib-metadata        | 7.1.0      | pypi_0             | pypi          |
| importlib-resources       | 6.4.0      | pypi_0             | pypi          |
| ipython                   | 8.12.3     | pypi_0             | pypi          |
| itsdangerous              | 2.1.2      | pypi_0             | pypi          |
| jedi                      | 0.19.1     | pypi_0             | pypi          |
| jinja2                    | 3.1.3      | pypi_0             | pypi          |
| keras                     | 2.10.0     | pypi_0             | pypi          |
| keras-preprocessing       | 1.1.2      | pypi_0             | pypi          |
| kiwisolver                | 1.4.5      | pypi_0             | pypi          |
| libclang                  | 18.1.1     | pypi_0             | pypi          |
| markdown                  | 3.6        | pypi_0             | pypi          |
| markupsafe                | 2.1.5      | pypi_0             | pypi          |
| matplotlib                | 3.7.5      | pypi_0             | pypi          |
| matplotlib-inline         | 0.1.6      | pypi_0             | pypi          |
| numpy                     | 1.24.3     | pypi_0             | pypi          |
| oauthlib                  | 3.2.2      | pypi_0             | pypi          |
| opencv-python             | 4.9.0.80   | pypi_0             | pypi          |
| openssl                   | 1.1.1w     | h2bbff1b_0         |               |
| opt-einsum                | 3.3.0      | pypi_0             | pypi          |
| packaging                 | 24.0       | pypi_0             | pypi          |
| parso                     | 0.8.3      | pypi_0             | pypi          |
| pickleshare               | 0.7.5      | pypi_0             | pypi          |
| pillow                    | 10.2.0     | pypi_0             | pypi          |
| pip                       | 23.3.1     | py38haa95532_0    |               |
| plumbum                   | 1.8.2      | pypi_0             | pypi          |
| prompt-toolkit            | 3.0.43     | pypi_0             | pypi          |
| protobuf                  | 3.19.6     | pypi_0             | pypi          |
| pure-eval                 | 0.2.2      | pypi_0             | pypi          |
| pyasn1                    | 0.5.1      | pypi_0             | pypi          |
| pyasn1-modules            | 0.3.0      | pypi_0             | pypi          |
| pygments                  | 2.17.2     | pypi_0             | pypi          |
| pyparsing                 | 3.1.2      | pypi_0             | pypi          |
| python                    | 3.8.0      | hff0d562_2        |               |
| python-dateutil           | 2.9.0.post0 | pypi_0            | pypi          |
| pywin32                   | 306        | pypi_0             | pypi          |
| requests                  | 2.31.0     | pypi_0             | pypi          |
| requests-oauthlib         | 1.4.0      | pypi_0             | pypi          |
| rsa                       | 4.9        | pypi_0             | pypi          |
| setuptools                | 68.2.2     | py38haa95532_0    |               |
| shapely                   | 2.0.3      | pypi_0             | pypi          |
| six                       | 1.16.0     | pypi_0             | pypi          |
| sqlite                    | 3.41.2     | h2bbff1b_0        |               |
| stack-data                | 0.6.3      | pypi_0             | pypi          |
| tensorboard               | 2.10.1     | pypi_0             | pypi          |
| tensorboard-data-server   | 0.6.1      | pypi_0             | pypi          |
| tensorboard-plugin-wit    | 1.8.1      | pypi_0             | pypi          |
| tensorflow                | 2.10.0     | pypi_0             | pypi          |
| tensorflow-estimator      | 2.10.0     | pypi_0             | pypi          |
| tensorflow-intel          | 2.13.0     | pypi_0             | pypi          |
| tensorflow-io-gcs-filesystem | 0.31.0  | pypi_0             | pypi          |
| termcolor                 | 2.4.0      | pypi_0             | pypi          |
| tf-slim                   | 1.1.0      | pypi_0             | pypi          |
| traitlets                 | 5.14.2     | pypi_0             | pypi          |
| typing-extensions         | 4.5.0      | pypi_0             | pypi          |
| urllib3                   | 2.2.1      | pypi_0             | pypi          |
| vc                        | 14.2       | h21ff451_1        |               |
| vs2015_runtime            | 14.27.29016 | h5e58377_2       |               |
| wcwidth                   | 0.2.13     | pypi_0             | pypi          |
| werkzeug                  | 3.0.1      | pypi_0             | pypi          |
| wheel                     | 0.41.2     | py38haa95532_0    |               |
| wrapt                     | 1.16.0     | pypi_0             | pypi          |
| zipp                      | 3.18.1     | pypi_0             | pypi          |
