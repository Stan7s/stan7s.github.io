学习一个数据分布，知道每一张图片

foward 映射到一个latentspace里

1. InferShape：接收一个ShapeInfo，经过神经网络变换之后的ShapeInfo
2. foward，_foward，_inverse
    _foward：将x映射成z，同时维护log(det_cobin) 即log(dz/dx)
    _inverse：将z映射成x，同时维护log(det_cobin) 即log(dz/dx)
    foward：包括以上两个（搞一个bool表示返回哪个）