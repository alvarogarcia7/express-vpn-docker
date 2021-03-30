# ExpressVPN Docker Setup

## Setup

Create a `.env` file [^0], containing:

[^0]: Suggested to copy from `.env.dist`.

```
$ cat .env
EXPRESSVPN_ACTIVATION_CODE=123
```

It is suggested to change your activation code instead of the sample value.

## Variants

The containers are available as branches on `containers/*`

## Running it

```
make run
```

In the logs, see:

```
expressvpn    | Restarting ExpressVPN service: expressvpnd.
expressvpn    | spawn expressvpn activate
expressvpn    | Enter activation code:
expressvpn    | Activating...
expressvpn    | Connected to $LOCATION
```

## Thanks

This project is based on [polkaned/dockerfiles](https://github.com/polkaned/dockerfiles/tree/master/expressvpn)
