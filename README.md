# aws-msb
Minimum security baseline
This is a set of cloudformation templates that deplpy a msb (minimum security baseline) in a new aws account that has no services enabled.
The cloudformation templates are part of a security program and should not be considered the only thing to do to improve your security posture in a new aws account.

Instructions:
- Create S3 bucket uin your AWS account
- upload the templates
   - root-stack.yml
   - plantilla-parametros.yml
   - plantilla-llaves.yml
   - plantilla-buckets.yml
   - plantilla-seguridad.yml
   - plantilla-notificaciones.ymkl
   
In AWS Cloudformation launch template root-stack.yml and provide parameters:
  - bucket-plantillas - ths is the name of the s3 bucket where the cloudformation templates are stored
  - abreviaturacuenta - this is an abreviation for your AWS account identification, it is used as part of the name on some of the created resources
  - correonotificacion - email to which the guardduty events notifications are sent
