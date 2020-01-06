# 3D 计算几何算法库(3D Compute Geometry Algorithm)

## 安装

```
npm install xtorcga -D
```

## 使用

- 全部引用;：

```javascript
import * as cga from "xtorcga";
function randomV3() {
  return cga.v3(
    Math.random() * 100 - 50,
    Math.random() * 100,
    Math.random() * 100 - 50
  );
}

var point = new cga.Point().copy(randomV3());
var seg = new cga.Segment(randomV3(), randomV3());
var result = point.distanceSegment(seg);
```

- 按需求引用：

```javascript
import { v3, Point, Segment } from "xtorcga";
function randomV3() {
  return v3(
    Math.random() * 100 - 50,
    Math.random() * 100,
    Math.random() * 100 - 50
  );
}

var point = new Point().copy(randomV3());
var seg = new Segment(randomV3(), randomV3());
var result = point.distanceSegment(seg);
```

-网页嵌入：直接使用 dist 下面的 cga.js

```html
<script src="./dist/cga.js" />
```

## 对象的类名

1. 点：**Point**
2. 直线：**Line**
3. 射线：**Ray**
4. 线段：**Segment**
5. 平面：**Plane**
6. 三角形：**Triangle**
7. 矩形：**Rectangle**

## 已经实现距离算法

√ 表示已经实现

? 表示将会实现

<!-- \- 表示对称 -->

× 表示不存在或者不实现

|        | 点  | 直线 | 射线 | 线段 | 平面 | 三角形 | 矩形 |
| :----: | :-: | :--: | :--: | :--: | :--: | :----: | :--: |
|   点   |  √  |  √   |  √   |  √   |  √   |   √    |  ?   |
|  直线  |  √  |  √   |  √   |  ?   |  ?   |   ?    |  ?   |
|  射线  |  √  |  √   |  √   |  √   |  ?   |   ?    |  ?   |
|  线段  |  √  |  ?   |  √   |  √   |  ?   |   ?    |  ?   |
|  平面  |  √  |  ?   |  ?   |  ?   |  ?   |   ?    |  ?   |
| 三角形 |  √  |  ?   |  ?   |  ?   |  ?   |   ?    |  ?   |
|  矩形  |  ?  |  ?   |  ?   |  ?   |  ?   |   ?    |  ?   |

## 展望

项目将会不断完善，如果你有好的想好可以提交你的想法。欢迎 star,让项目更进一步

## 讨论

QQ 群：469014839