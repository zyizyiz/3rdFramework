# 3rdFramework
1. ### SDWebImage

   调用方法：

   | 方法                                              |                                                              |      |
   | ------------------------------------------------- | ------------------------------------------------------------ | ---- |
   | sd_setImageWithURL                                |                                                              |      |
   | sd_internalSetImageWithURL（UIView+WebCache类）   | 根据operationKey获取字典中的value取消加载图片的操作，然后设置关联对象，根据SDWebImageOptions异步做一些设置图片的操作，然后如果url不为空，则设置actiivtyIndicator指示器，最后获取SDWebImageManager单例，执行loadImageWithURL方法 |      |
   | loadImageWithURL（SDWebImageManager类）           | 调用queryCacheOprationForkey                                 |      |
   | queryCacheOperationForKey（SDImageCache类）       | 首先从imageFromMemoryCacheForKey中查找图片，其次diskImageDataBySearchingAllPathsForKey从磁盘中查找图片NSData，然后根据找到的NSData调用diskImageForKey解档为Image图片并做一些尺寸处理，然后将图片存在内存中 |      |
   | downloadImageWithURL（SDWebImageDownloadToken类） | 调用createDownloaderOperationWithUrl进行图片下载             |      |
   | storeImage（SDImageCache类）                      | 存储图片到内存中，并归档为NSData存储                         |      |
   |                                                   |                                                              |      |
   |                                                   |                                                              |      |
   |                                                   |                                                              |      |

   

2. 

3. 

4. 

5. 

