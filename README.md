>
	--初始化变量
	local M = {}
	M.imagevarobj = require("image.imagevar")
	M.imagevarobj.init()
	M.imagevar = M.imagevarobj.image
	--图片处理
		--M.imagevar变量参数集
		--local_file_cachedir缓存目录
		--local_file_cachepath缓存文件
		--fun 功能函数库
	local ImageConfig = {}
	local gmagick = require("image.gmagick").new(M.imagevar,img.config.local_file_cachedir,img.config.local_file_cachepath,fun)
	gmagick.run()
