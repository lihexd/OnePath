# Tizen-App-OnePath

## 概述

 OnePath是一款益智游戏，游戏规则非常简单。根据所给出的图形，确定一个好的起点，然后连接所有点，但是不能重复覆盖每一条边。现在这款游戏只有60张图，难度分为容易，中等，难。每通过一个关卡，系统会根据时间长短来评分，三颗星即为满分。注意哦，越往后游戏难度将会越大。
## 算法介绍

OnePath基于TIZEN web project开发，主要使用了Html与Javascript技术。```js
onclick: function(a, b) {
			var 
			f = this,
			g = a / f.dh,
			h = b / f.dh;
			if (f.aJ.click(g, h)) return tq;
			if (f.u0 || f.qw) return;
			if (f.qw) {
				f.sL(f.level),
				f.qw = tq;
				return
			}
			c = f.uA(g, h);
			if (c == UD) return;
			d = f.pN(c);
			if (f.Y2d1 != UD) {
				e = f.U7(f.Y2d1, c);
				if (e == UD) {
					if (f.Y2d1.x == c.x && f.Y2d1.y == c.y) return;
					f.aS = {
						l: {
							p: [{
								x: f.Y2d1.x,
								y: f.Y2d1.y,
								t: 0
							},
							{
								x: c.x,
								y: c.y,
								t: 1
							}]
						},
						ds: [{
							x: f.Y2d1.x,
							y: f.Y2d1.y
						},
						{
							x: c.x,
							y: c.y
						}]
					},
					f.po();
					return
				}
				f.zw = a1,
				e.selected = a1,
				f.pl(e),
				f.cr.Uds(e, c),
				f.Y2d1.selected = tq,
				f.zJ(f.Y2d1);
				if (f.zQ()) {
					c.selected = a1,
					f.zJ(c),
					f.pw(),
					f.Ger.us(d, 5, 35, 30, 3, 700, 19, new qg(255, 210, 132)),
					f.Ger.us(d, 20, 65, 30, 3, 600, 19, new qg(255, 210, 132)),
					f.Ger.us(d, 30, 95, 90, 3, 400, 19, new qg(255, 210, 132)),
					c.selected = a1;
					return
				}
			}
			c.selected = a1,
			f.zJ(c),
			f.Y2d1 = c,
			f.Ger.us(d, 10, 45, 30, 3, 600, 25, new qg(255, 255, 255))
		},//点击激活节点
	```
