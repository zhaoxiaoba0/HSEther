# HSEther ether wallet create 



<img src="https://github.com/wolfhous/HSEther/blob/master/seedemo.gif" width="300" hegiht="420" align=center />

<img src="https://upload-images.jianshu.io/upload_images/2923333-3d96e2eb2a0d2df6.png" width="900" hegiht="420" align=center />

## 您的star是我最大的动力

### 1.0 临时主要功能（2018-04-20）：

* 1.0.1 离线创建钱包 生成对应算法助记词、私钥、keystore（生成钱包

* 1.0.2 验证钱包keystore和密码 （keystore导入钱包

* 1.0.3 验证私钥（私钥导入钱包

* 1.0.4 验证助记词（助记词导入钱包

**以上安全起见，不调用接口实现，全部本地离线验证。**


### 1.1 主要添加功能（2018-05-07）：

* 1.1.1 查询以太坊余额

* 1.1.2 查询基于以太坊公链token代币余额（ERC20代币余额）

### 1.2 主要添加功能（2018-06-05）：

* 1.2.1 以太坊转账

* 1.2.2 基于以太坊token的代币（ERC20代币）转账（比如EOS转账等）

### 1.3 主要添加功能（预计完成2018-06-30）：

* 1.3.1 ERC20代币 总量查询

* 1.3.2 ERC20代币 官方图标查询

* 1.3.3 ERC20代币 小数位数查询...等等...

### 1.4 主要添加功能（预计完成2018-07）：

* 1.4.1 **自定义发行ERC20代币**



------------------------------------------------
# 支持 cocoaPods
```
# ios version 10.0+
cocoaPods HSEther
```

------------------------------------------------
# 具体用法 详见Demo
```
 [1]创建钱包

+(void)hs_createWithPwd:(NSString *)pwd block:(void(^)()block;
                  
 [2]助记词导入
 
+(void)hs_inportMnemonics:(NSString *)mnemonics pwd:(NSString *)pwd block:(void(^)()block;

 [3]KeyStore 导入
 
+(void)hs_importKeyStore:(NSString *)keyStore pwd:(NSString *)pwd block:(void(^)()block;

 [4]私钥导入

+(void)hs_importWalletForPrivateKey:(NSString *)privateKey pwd:(NSString *)pwd block:(void(^)()block;


 [5]查询eth和代币余额

+(void)hs_getBalanceWithTokens:(NSArray<NSString *> *)arrayToken
                   withAddress:(NSString *)address
                         block:(void(^)(NSArray *arrayBanlance,BOOL suc))block;
                         
 [6]转账
 
+(void)hs_sendToAssress:(NSString *)toAddress 
                  money:(NSString *)money 
               tokenETH:(NSString *)tokenETH 
                decimal:(NSString *)decimal 
        currentKeyStore:(NSString *)keyStore 
                    pwd:(NSString *)pwd 
               gasPrice:(NSString *)gasPrice 
               gasLimit:(NSString *)gasLimit 
                  block:(void(^)(NSString *hashStr,BOOL suc,HSWalletError error))block;
  ```                            
                              

------------------------------------------------
## 提供 非静态库源码，包括iOS和Android
## 提供 技术支持，包括iOS和Android
## 联系wechat： iHoushuai
------------------------------------------------
简书地址：https://www.jianshu.com/p/6839a8c3f220
------------------------------------------------
