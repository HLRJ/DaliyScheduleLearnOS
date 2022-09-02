# Day02

## 进度

- [x] 完成三个exercise

| Exercise        |
|-----------------|
| move_semantics  |
| primitive_types |
| structs         |


进度图

![三个练习](/photos/day02/day02_00.png) 


## 细节

move_semantics2：   
```1. Make another, separate version of the data that's in `vec0` and pass that
to `fill_vec` instead.
2. Make `fill_vec` borrow its argument instead of taking ownership of it,
   and then copy the data within the function in order to return an owned
   `Vec<i32>`
3. Make `fill_vec` *mutably* borrow its argument (which will need to be
   mutable), modify it directly, then not return anything. Then you can get rid
   of `vec1` entirely -- note that this will change what gets printed by the
   first `println!```

`vec0  ==>  fill_vec(vec0.clone())`

move_semantics2 和 move_semantics3 的区别在于 
println! 一个是打印vec0和vec1 一个是打印vec1两次

做了三个exercises，感觉在 `move_semantics` ， 借用所有权，可变不可变，有点绕。