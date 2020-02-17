# gwf
增加流媒体视频域名列表

使用条件和方法

1、你使用的是L大的LEDE固件，内部有SSR PLUS+这个插件
2、将gwf.list覆盖到路由器/etc/config/

推荐ssh工具 MobaXterm 

备注：
如果你使用的是SSR PLUS+ 你还可以用另外一种简便方法，在访问控制--强制走代理的域名中添加Netflix相关域名即可。另外如果你使用视频的方法，你修改了gfw.list 之后，还是不行，你可以尝试重启电视盒子。按理说 应该清理下DNS缓存，但是电视盒子清理dns缓存不好弄，干脆断电重启下电视盒子。如果是电脑的在替换后的gfwlist模式下访问不了Netflix 你直接在命令行清除dns缓存就行。ipconfig /flushdns 。还有就是有的观众的固件可能原本在/etc/config/下根本没有gfw.list文件 ，这种情况 就别往里拖拽了，肯定不存在这种机制，应该不管用，估计是ssr plus+ 没有安装或者版本不同。

参考网站：https://fuyiyi.imdo.co/articles/2018/10/26/1540532958285.html#b3_solo_h3_7
