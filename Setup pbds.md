### Steps
1) First, go to this location -> C:\MinGW\lib\gcc\mingw32\6.3.0\include\c++\ext\pb_ds\detail\resize_policy
2) There you will see a file similar to -> "hash_standard_resize_policy_imp.hpp0000644". Rename it to "hash_standard_resize_policy_imp.hpp" . 
3) Add these lines in your code: <br>
   #include <ext/pb_ds/tree_policy.hpp> <br>
   #include <ext/pb_ds/assoc_container.hpp> <br>
   using namespace __gnu_pbds; <br>
   template <typename T>  using ordered_set = tree<T, null_type, less<T>, rb_tree_tag, tree_order_statistics_node_update>; <br>
   
   That's all!
