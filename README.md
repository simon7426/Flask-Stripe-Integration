# Flask Stripe Integration

This project does a POC of integrating Flask with Stripe. This was done using following the blog by [Michael Herman](https://testdriven.io/blog/flask-stripe-tutorial/)

## Using the project

- Install the dependencies

```console
poetry install
```

- Add your Stripe test secret and publishable keys as environment variables

```console
export STRIPE_PUBLISHABLE_KEY=<STRIPE_PUBLISHABLE_KEY>
export STRIPE_SECRET_KEY=<STRIPE_SECRET_KEY>
```

- To confirm payments using webhooks, add the webhook endpoint environment variable

```console
export STRIPE_ENDPOINT_SECRET=<ENDPOINT_SECRET_KEY>
```

- Run the server

```console
FLASK_DEBUG=1 poetry run python app.py
```

Navigate to <http://localhost:5000>
