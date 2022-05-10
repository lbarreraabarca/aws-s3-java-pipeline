# aws-s3-java-pipeline


## Contract

```json
{
    "s3Operator": {
        "landingPath": "s3://my-bucket/test/data.csv",
        "localPath": "/my-local-path/data.csv",
        "bucketRegion": "us-west-1"
    } 
}
```

## Environment Variables

```
export ENV_AWS_KEY_ID=[AWS_KEY_ID]
export ENV_AWS_ACCESS_KEY=[AWS_ACCESS_KEY]
export ENV_INPUT_CONTRACT=ewogICAgInMzT3BlcmF0b3IiOiB7CiAgICAgICAgImxhbmRpbmdQYXRoIjogInMzOi8vbXktYnVja2V0L3Rlc3QvZGF0YS5jc3YiLAogICAgICAgICJsb2NhbFBhdGgiOiAiL215LWxvY2FsLXBhdGgvZGF0YS5jc3YiLAogICAgICAgICJidWNrZXRSZWdpb24iOiAidXMtd2VzdC0xIgogICAgfSAKfQ==
```

## How to use ?
```bash
mvn clean package -DskipTests
java -jar target/aws_s3_java_pipeline-1.0.jar
```