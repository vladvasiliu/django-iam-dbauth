# Django IAM database backends

## Usage

    pip install django-iam-dbauth

In your settings use the following

    DATABASES = {
        "default": {
            "HOST": "<hostname>",
            "USER": "<user>",
            "ENGINE": 'django_iam_dbauth.aws.postgresql'
        }
    }


# Caveats

1. You cannot use a cname for the host, it needs to be the actual hostname of
the RDS instance.
