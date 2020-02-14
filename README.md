**AWS EC2 Instance Terraform light module**

**A simple EC2 instance module for Terraform.**

**Usage**

module &quot;ec2\_instance&quot; {

source                 = &quot;github.com/fopingn/terraform-aws-instance-basic.git&quot;

  version                = &quot;~\&gt; 2.0&quot;

  name                   = &quot;my-cluster&quot;

  instance\_count         = 5

  ami                    = &quot;ami-ebd02392&quot;

  instance\_type          = &quot;t2.micro&quot;

  key\_name               = &quot;user1&quot;

  monitoring             = true

  vpc\_security\_group\_ids = [&quot;sg-12345678&quot;]

  subnet\_id              = &quot;subnet-eddcdzz4&quot;

  tags = {

    Terraform   = XXXX

    Environment = XXXX

  }

Note: You have to give several values to tag in all above tags

## License

MIT
