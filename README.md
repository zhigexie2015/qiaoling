# qiaoling
 巧灵脑筋急转弯大模型（基于yuan2.0-2B模型微调）

部署方法

1.下载llama factory代码。https://github.com/hiyouga/LLaMA-Factory
 
2.安装相关依赖，安装llama factory相关命令。 

3.下载yuan2.0-2B-Mars-hf模型，https://modelscope.cn/models/IEITYuan/Yuan2-2B-Mars-hf/files  里面的所有文件，存储到本机。

4.下载本仓库./LoraCheckPoints 里面的所有文件，存储到本机。

5.将推理配置文件yuan2b_lora_sft.yaml拷贝到./LLaMA-Factory/examples/inference/。修改Lora的路径和yuan2.0-2B的路径为本机路径。

6.运行推理命令llamafactory-cli webchat examples/inference/yuan2b_lora_sft.yaml。 

7.默认在本机浏览器打开http://0.0.0.0:7860/，  即可进行脑筋急转弯问答。

#源2.0大模型简介  

源2.0 是浪潮信息发布的全新一代基础语言大模型系列，包含源2.0-102B、源2.0-51B 和源2.0-2B。基于源1.0，源2.0 利用更多样的高质量预训练数据和指令微调数据集，显著提升了模型在语义理解、数学推理、代码生成和知识获取等方面的能力。我们提供了全套预训练、微调和推理服务的脚本，支持研发人员进行深度开发。
