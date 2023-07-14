# Add feature: Delete the image associated with a todo item when deleting the item.

## serveless.yaml
```
# add S3:deleteObject policy

https://github.com/kydq2022/05-capstone-project/blob/master/backend/serverless.yml#L247

# To provide an IAM role for deleting S3 objects in a Lambda function

https://github.com/kydq2022/05-capstone-project/blob/master/backend/serverless.yml#L126-L129

```
## fileStorage
```

https://github.com/kydq2022/05-capstone-project/blob/master/backend/src/fileStorage/attachmentUtils.ts#L32-L43`


```

## businessLogic
```
## Call function to delete an S3 object when deleting a todo item
https://github.com/kydq2022/05-capstone-project/blob/master/backend/src/businessLogic/todos.ts#L72-L76

```

# Testing

## On Client
![Alt text](images/client.png?raw=true "Image 1")

## S3
![Alt text](images/s3.jpeg?raw=true "Image 1")

## Click on 'x' to delete todo item

![Alt text](images/client2.png?raw=true "Image 2")

## Verify on S3, the associated image is also removed.
![Alt text](images/s3-2.jpeg?raw=true "Image 1")