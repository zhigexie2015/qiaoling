# qiaoling
 巧灵脑筋急转弯大模型-基于yuan-2模型LORA微调后的脑筋急转弯大模型

部署方法

1.下载llama factory代码。https://github.com/hiyouga/LLaMA-Factory
 
2.安装相关依赖，安装llama factory相关命令。 享

3.下载源yuan2.0-2B-Mars-hf模型，https://modelscope.cn/models/IEITYuan/Yuan2-2B-Mars-hf/files里面的所有文件，存储到本机。

4.下载本仓库./LoraCheckPoints 里面的所有文件，存储到本机。

4.将推理配置文件yuan2b_lora_sft.yaml拷贝到./LLaMA-Factory/examples/inference/。修改Lora的路径和yuan2.0-2B的路径为本机路径。

5.运行推理命令llamafactory-cli webchat examples/inference/yuan2b_lora_sft.yaml。 

6.默认在本机浏览器打开http://0.0.0.0:7860/，即可进行脑筋急转弯问答。
