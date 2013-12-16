UIImageView-AFNetworking-OneByOneQueue
======================================

New parameter added for UIImageView+AFNetworking methods by simply adding a new NSOperationQueue instance. 

* \- (void)setImageWithURL:(NSURL *)url **oneByOne:(BOOL)isOneByOne**;  

* \- (void)setImageWithURL:(NSURL *)url
       placeholderImage:(UIImage *)placeholderImage
               **oneByOne:(BOOL)isOneByOne**;  
               

* \- (void)setImageWithURLRequest:(NSURLRequest *)urlRequest
              placeholderImage:(UIImage *)placeholderImage success:(void (^)(NSURLRequest *request, NSHTTPURLResponse *response, UIImage *image))success failure:(void (^)(NSURLRequest *request, NSHTTPURLResponse *response, NSError *error))failure **oneByOne:(BOOL)isOneByOne**;

##When to?
As you wish.

##How to?
Simply replace the files in AFNetworking sources.  

##Example
[cell.avatarView setImageWithURL:[NSURL URLWithString:@"http://www.qqtouxiang888.com/uploads/allimg/110322/093310AU-2.jpg"] **oneByOne:YES**];
