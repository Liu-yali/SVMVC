# SVMVC文件相关说明
该文件是论文（具有分存验证功能的多色调可视密码）的部分实验结果图像。
论文提出方案名称：Shares Verification Multitone Visual Cryptography，简称SVMVC。

大致简介：提出基于一组互补子模式且具有分存验证功能的多色调可视密码。编码时，首先将原始灰度图像转化为多色调图像；其次利用DPI（Dots Per Inch）与PPI（Pixels Per Inch）间不对等的关系，设计一组自带权重且互补的子模式，将多色调图像分解为多个二值位平面；最后依据二值可视密码的编码规则，将位平面编码为独立位平面分存。为了便于管理者管理分存，将独立位平面分存进行位平面累加运算转换为多色调分存。解码前，分存验证模块进行分存验证，若验证某分存为真，则该分存参与解码。解码时，将同级位平面分存堆叠得到各个重建位平面；堆叠所有的重建位平面解码出原始灰度图像。本方案具有分存验证功能且解码无需计算。实验结果表明本文重建的图像质量优于其它方案。
Fig.10：为本文的两组以独立位平面形式存放的分存图像，数制为二进制。

Fig.11：将Fig.10经为位平面累加运算后得到的多色调分存。由于选用的子模式权重为8、4、2、1，因此Fig.11中的数据值在0-15之间。

Fig.13：为本文的两组以独立位平面形式存放的验证分存图像，数制为二进制。
