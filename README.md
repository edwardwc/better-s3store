# S3Store

S3Store is a storage module that uses Amazon's S3 object storage as a [storage interface](https://github.com/caddyserver/certmagic/wiki/Storage-Implementations) for [CertMagic](https://github.com/caddyserver/certmagic).

## Usage

The `NewS3Storage(bucket, region string)` function will automatically use credentials from ENV vars, `~/.aws/credentials` files and any assumed roles.
It should not be necessary to provide any explicit credentials.

Otherwise, if you want to provide explicit credentials, you can do so with `NewS3StorageWithCredentials(accessKey, secretKey, bucket, region string)`.

## License

This library is distributed under the [MIT License](https://opensource.org/licenses/MIT), see [LICENSE](https://github.com/aymanbagabas/s3store/blob/master/LICENSE) for more information.