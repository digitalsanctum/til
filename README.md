# til
Today I Learned

## June 2, 2020
* [Nix](https://nixos.wiki/wiki/Nix) - a package manager and build system that parses reproducible build instructions specified in the Nix Expression Language, a pure functional language with lazy evaluation. 
* There are 3-4 implementations in mainstream use: nawk (the one true awk, an ancient version of which is installed on Mac OS by default), mawk (installed on eg. Ubuntu by default), gawk (on RH by default last I checked), or busybox-awk. Tip: mawk is much faster than the others and to get performance out of gawk you should use LANG=C (and also because of crashes with complex regexpes in Unicode locales in some versions of gawk 3 and 4).
* [xstate](https://xstate.js.org/docs/) - JavaScript and TypeScript finite state machines and statecharts.
* [shadowenv](https://github.com/Shopify/shadowenv) - reversible directory-local environment variable manipulations.
* [envsubst](https://www.gnu.org/software/gettext/manual/html_node/envsubst-Invocation.html) - substitutes the values of environment variables.

```
FOO=foo
BAR=bar
export FOO BAR

envsubst <<EOF
FOO is $FOO
BAR is $BAR
EOF
```

## May 11, 2020
* [Kubernetes GC](https://kubernetes.io/docs/concepts/workloads/controllers/garbage-collection/) - by default, once disk usage is 80% the GC will delete container images.

## May 7, 2020
* [Language Server Protocol](https://microsoft.github.io/language-server-protocol/)

## May 6, 2020
* `docker system prune`
* [exa](https://the.exa.website/) - modern replacement for `ls` written in Rust.

## May 5, 2020
* [GOTO 2019 • "Good Enough" Architecture • Stefan Tilkov](https://www.youtube.com/watch?v=PzEox3szeRc)
   * [ISO/IEC/IEEE 42010 Systems and software engineering](https://en.wikipedia.org/wiki/ISO/IEC_42010)
   * Standardization vs. Autonomy - there must be a balance between the two.
   * Centralization - hurts; become a bottle neck.
   * There's a fine line between diversity (that adds value) and chaos (that doesn't add value).
   * Loose coupling requires very few rules, but they need to be enforced strictly.
* [Add enriched metadata to Amazon VPC flow logs published to CloudWatch Logs and S3](https://aws.amazon.com/about-aws/whats-new/2020/05/add-enriched-metadata-to-amazon-vpc-flow-logs-published-to-cloudwatch-logs-and-s3/)
