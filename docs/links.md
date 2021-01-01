## Site with instructions for setting up Jupyter on EC2: https://dataschool.com/data-modeling-101/running-jupyter-notebook-on-an-ec2-server/

## code added to jupyter config

```python
conf = get_config()

conf.NotebookApp.ip = '0.0.0.0'
conf.NotebookApp.password = u'sha1:d4dac6a21fc1:1c09038894a992aeb7cd4b299fa019086daa008e'
conf.NotebookApp.port = 9161
```

Next step: Create an image that can be reused

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/creating-an-ami-ebs.html

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/RootDeviceStorage.html

https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ComponentsAMIs.html#storage-for-the-root-device

