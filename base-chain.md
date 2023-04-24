# Base chain 空投教程

### 前置准备
* Metamask小狐狸钱包。（可以用Firefox浏览器装metamask插件，生成钱包后手机app上下载metamask并导入钱包。）
* [chainlist](https://chainlist.org/)网站上搜索 $\color{#0000FF}{Goerli}$ 测试链， $\color{#0000FF}{Base}$ 测试链和 $\color{#FF0000}{Optimism}$ L2侧链。并添加至钱包。
* twitter账户。

### 任务1：四大 NFT mint
* 钱包切换 $\color{#00FFF}{以太坊}$ 主链。去[官网](https://mint.base.org/)mint第一个nft。
* 钱包切换 $\color{#FF0000}{Optimism}$ L2侧链。去[博客](https://base.mirror.xyz/H_KPwV31M7OJT-THUnU7wYjOF16Sy7aWvaEr5cgHi8I)文章最下面mint第二个nft。
* 钱包依然在 $\color{#FF0000}{Optimism}$ L2侧链。去[博客](https://base.mirror.xyz/nft/0x0856c0E5DDCfC71Ad07D765ddCabAc0eac5b283a/0)文章最下面mint第三个nft。
* 钱包切换 $\color{#00FFF}{以太坊}$ 主链。去[网站](https://zora.co/collect/0x554f3b93d82ce2435206f3ad8ac4154d056cd18e)mint第四个nft。

### 任务2：Base 测试链存入提取 ETH 交互
* 钱包切换 $\color{#0000FF}{Goerli}$ 测试链。去[quicknode](https://faucet.quicknode.com/drip)领水。
* 去[官方桥](https://bridge.base.org/deposit)。输入 $\color{#0000FF}{Goerli}$ 测试链一半的eth后点击 [DEPOSIT ETH] 按钮。钱包切换 $\color{#0000FF}{Base}$ 测试链等ETH到账后，再在官方桥点Withdraw标签页，输入一半的ETH后点击 [WITHDRAW] 按钮。

### 任务3：Base 测试链部署 NFT 任务交互
* 钱包切换 $\color{#0000FF}{Base}$ 测试链。去[thirdweb](https://thirdweb.com/thirdweb.eth/DropERC721)部署合约，打开页面后点击右边 [Deploy now] 按钮，在跳出来的弹框里的name输入框里随便输入一个name（比如symbol）即可，页面滑动到最下面点击 [Deploy Now] 按钮，等钱包跳出弹框（2次）点击确认。等待合约部署完成。
* 合约部署完成后，复制合约name（比如symbol）下面的地址（address）。去[quest](https://quests.base.org)页面connect钱包 $\color{#FF0000}{（这里可能是防女巫，现在需要手机metamask钱包扫码链接）}$ 点击 [Start Quest] 按钮一路 [continue] 最后在 [Smart contract address] 输入框内粘贴复制好的合约地址。点解 [VERIFY TRANSACTION]按钮一路 [continue] 跳转到NFT页面点击 [MINT NFT] 按钮，等手机钱包跳出签名按钮点击确认即可。

### 任务4：Base 测试链部署 TOKEN 合约交互
* 钱包切换 $\color{#0000FF}{Base}$ 测试链。打开[在线合约](https://remix.ethereum.org/)编辑网站，在左边default_workspace工程下的contracts目录下新建token合约文件_Token_airdrop.sol并将[base_chain_files](https://github.com/ccenlei/airdrops/tree/main/base_chain_files)目录下同名的文件的代码拷贝进去。
* 点击remix左侧栏第四个 [Solidity compiler] 按钮编译合约。
* 点击remix左侧栏第五个 [Deploy & run transactions] 按钮运行合约，Environment框选择 [Injected Provider - Metamask] 连接钱包，在account栏确认地址和余额是否正确。点击 [Deploy] 按钮并在钱包跳出的弹框里点确认即可。

### 任务5：Base 测试链 Kitten 交互
* 钱包切换 $\color{#0000FF}{Base}$ 测试链。打开[catattacknft](https://catattacknft.vercel.app/)网站。连接钱包，点击 [Claim Kitten] 按钮，在钱包弹出框点击确认即可。
* claim 成功后点击 [transfer] 按钮随便选中一个player点击transfer。在钱包弹出框里点击确认。
* 剩下的玩法自行探索，目标就是刷交互量。

### 任务6：Base 测试链 Cbswap 交互
* 钱包切换 $\color{#0000FF}{Base}$ 测试链。打开[cbswap](https://app.cbswap.io/#/swap)网站。连接钱包，交互 兑换(swap)功能和流动池(liquidity)功能即可。

### 备注：任务5和任务6可以每天或每n天交互n次，刷transactions交易量。
