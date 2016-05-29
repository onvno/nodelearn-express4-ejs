# nodelearn-express4-ejs
针对之前express3小实例做的迁移

参照expressjs官方指导，同时SO解决些小问题。

以下命令需要删除才正常执行,需要之后深入了解node时再做进一步解释

	var multer = require('multer');
	app.use(multer());

以下已废弃，4.0有新的route加入

	app.use(app.router);

中间件需要自行加载引入

	var express = require('express');
	var path = require('path');
	var http = require('http');
	var favicon = require('serve-favicon');
	var logger = require('morgan');
	var cookieParser = require('cookie-parser');
	var bodyParser = require('body-parser');
	var methodOverride = require('method-override');
	var partials = require('express-partials');
	// var multer = require('multer');
	var errorHandler = require('errorhandler');
	var routes = require('./routes');