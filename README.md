# Filesystem-Implementation
Instagram clone: Files can be uploaded and comments can be added to any of the file.
 purpose: 
      managing pictures(uploading &amp; downloading) along with their comments given by other users.
      The data will be stored as user specific data , so we can track the user progress and getdata as per user.
Basic Information:
      developed using C  capacity: 100mb(expandable to even GBs of data) 
  
Other Information about implementation:
      FIle size --> 104857600 ->100MB
      BLOCK SIZE 128 bytes
      FILE BLOCK SIZE 2048
      Master block 1 block
      Bit vector 1280 blocks 128 * 1280 = 163,840 bytes
      Users data 1281 block num to 7sb complete next start from 1297th block

      Meta message 1297 block no start total 8192 + 8192 blocks reserved
      Message data 17681 block no start total 8192 + 8192 blocks reserved
      
      File metadata 34065 block no start total	// 128 -> 2kb(2048bytes) block size // total 7082 blocks leaving 112 bytes atlast
      

optimizations: 
      Bit-vector implementation for effective use of memory.User can upload, download and can delete the data also he can keep track of comments made by other users.
    
