# tm_onboarding_gcf

TerraMagna cloud functions onboarding challenge.

## HTTP

Commands used on deploy:
```console
$ cd http
$ gcloud functions deploy onboarding_jv_http --runtime python39 --trigger-http --allow-unauthenticated
```

How to test it:
https://us-central1-tm-devops-labs.cloudfunctions.net/onboarding_jv_http?name=GitHub

## Pub/Sub

Commands used on deploy:
```console
$ cd pubsub
$ gcloud pubsub topics create ONBOARDING_JV_TOPIC
$ gcloud functions deploy onboarding_jv_pubsub --trigger-topic ONBOARDING_JV_TOPIC --runtime python39
```

How to test it:
```console
$ gcloud pubsub topics publish ONBOARDING_JV_TOPIC --message="GitHub"
```



CONGRATS BRO! YOU ROCK IT! 

NEXT WEEK WE'LL TALK ABOUT TERRAFORM AND HOW CAN YOU DO IT USING INFRASTRUCTURE AS A CODE!

SEE YOU SOON!

HAVE A NICE WEEKEND!
