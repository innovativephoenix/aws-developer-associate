# What is Versioning?

1. Versioning is a means for keeping multiple variants of the same object in the bucket.

1. Versioning is used to preserve, retrieve, and restore every version of every object stored in an S3 bucket.

1. Versioning is done at the S3 Bucket level.

1. Versioning can be enabled from the AWS Console / SDKs / API.

1. Versioning, once enabled, cannot be completely disabled.


## The Alternative

- The alternative to disabling versioning is placing the bucket in a "versioning-suspended" state.

- A drawback of having multiple versions of an object is you are billed multiple times (since the objects are getting stored in S3 each time).

- In order to avoid having multiple versions of the same object, S3 has a feature called Lifecycle  Management. This allows us to decide on what to do when multiple versions of an object are piling up.

- One advantage of versioning is, we can provide permissions on versioned objects i.e., we can define which version of an object is public and which one is private.

## Task Details

1. Log into the AWS Management Console.
1. Create an S3 bucket.
1. Enable object versioning on the bucket.
1. Upload a text file to the S3 Bucket.
1. Test object versioning by changing the text file and re-uploading it.

