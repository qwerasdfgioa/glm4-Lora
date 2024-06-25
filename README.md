# glm4-Lora
基于glm-4-9b-chat的Lora微调
使用本地的医疗问答的一个数据集大概两万多条问答记录，提供了半精度训练和4bit量化的两个Lora微调代码示例

将glm-4模型下载到当前文件夹下即可
!git lfs clone http://huggingface.co/THUDM/glm-4-9b-chat

使用半精度训练max_length设置为256，batch设置为2，梯度累加为8，打开梯度检查点，Lora微调大概需要22G显存；

使用4bit量化max_length设置为768，batch设置为1，梯度嘞家为16，开启梯度检查点，Lora微调大概需要18G显存；
