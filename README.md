AFNetworking-AutoRetry
======================

An iOS category adding retry functionality to requests made using AFNetworking 2.X


#import "AFHTTPRequestOperationManager+AutoRetry.h"

// this will retry the request 3 times, will wait 0.5 second before retry, each time
AFHTTPRequestOperation *operation = [self.manager HTTPRequestOperationWithRequest:request
                                                                          success:success
                                                                          failure:failure
                                                                      autoRetryOf:3
                                                                    retryInterval:0.5f];

