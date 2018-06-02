# Azeria

### What is this?

This is a social microblogging application. If you've heard of Mastodon, this is almost exactly like it, only it's written with 
performance and memory in mind, and a few other features that Glitch-Soc's fork of Mastodon has.

### What's an Azeria?

It's the word "fox" in Basque. But it also represents me trying to rewrite Mastodon in such a way that it will be faster.

### Why a fox?

Mastodon is elephant-like mammal, but I can make a comparison to the elephant, right? The African elephant runs at 24.9 km/h (15.5 
mph) while the red fox runs at 49.9 km/h (31 mph). Therefore, faster. Have I mentioned [foxes are awesome](https://static.boredpanda.com/blog/wp-content/uploads/2014/03/amazing-fox-photos-5.jpg)?

### Okay, why faster?

My goals for this project:

1. Write the backend targeting Python 3.5.3 and run it with PyPy. Be as performant on a server with 10,000 users as it is with 10. (It was either this or Go, and I really needed to unrust my Python.)
1. Re-write the frontend a bit, but keep React. Frontend will be served via Flask.
1. Use Argon2 password hashing and force TLS 1.2 *or, even better* TLS v1.3 for transportation methods between hosted servers.
1. Try to improve user discovery methods and federation, while trying to verify users on other hosted servers.
1. Support U2F (Yubikey, etc.) authentication.
1. Use DNSCrypt, though this will be off by default and optional.
1. Add in [glitch-soc specific](https://glitch-soc.github.io/docs/) features while adding more often-requested features.
1. Use Docker as it will make deployment and upgrading a lot easier.
1. Not run into trouble with Docker's lack of IPv6. (Yep, using ipv6nat container.)
1. Use Nginx combined with [acme.sh](https://acme.sh) to deploy a frontend that uses modern cipher suites and protocols.
1. Try to be as open as possible from suggestions and constructive feedback. Have a good Code of Conduct.
1. **Be as easy to setup and as easy to run as possible.**

### This project is empty. What next?

Working on it~
