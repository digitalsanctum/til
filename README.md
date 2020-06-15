# til
Today I Learned

## June 15, 2020
* [rook](https://rook.io/) - open-source, cloud-native storage for Kubernetes. Rook orchestrates multiple storage solutions, each with a specialized Kubernetes Operator to automate management. Choose the best storage provider for your scenarios, and Rook ensures that they all run well on Kubernetes with the same, consistent experience.
* [sealed secrets](https://github.com/bitnami-labs/sealed-secrets) - a Kubernetes controller and tool for one-way encrypted Secrets.

## June 12, 2020
* [nats](https://nats.io/) - a simple, secure and high performance open source messaging system for cloud native applications, IoT messaging, and microservices architectures.
* [dapr](https://dapr.io/) - distributed application runtime built on nats.

## June 10, 2020
* [GOTO 2020 • What We Left Behind - 10 Valuable Skills From The 1990s • Garth Gilmour & Eamonn Boyle](https://www.youtube.com/watch?v=DrBPXSiUWbI)
* [GOTO 2020 • Beyond Microservices: Streams, State and Scalability • Gwen Shapira](https://www.youtube.com/watch?v=H0LUi51aCP8)

## June 9, 2020
* 432 Hz vs. 440 Hz Tuning Standards

## June 7, 2020
* [Temporal workflow vs Cadence workflow](https://stackoverflow.com/questions/61157400/temporal-workflow-vs-cadence-workflow) - explaination of the differences by the original tech lead of both.
* [Cadence Workflow](https://cadenceworkflow.io/) - a fault-oblivious stateful programming model that obscures most of the complexities of building scalable distributed applications. In essence, Cadence provides a durable virtual memory that is not linked to a specific process, and preserves the full application state, including function stacks, with local variables across all sorts of host and software failures. This allows you to write code using the full power of a programming language while Cadence takes care of durability, availability, and scalability of the application.
* [Saga Pattern](https://microservices.io/patterns/data/saga.html) - Implement each business transaction that spans multiple services as a saga. A saga is a sequence of local transactions. Each local transaction updates the database and publishes a message or event to trigger the next local transaction in the saga. If a local transaction fails because it violates a business rule then the saga executes a series of compensating transactions that undo the changes that were made by the preceding local transactions.


## June 4, 2020
* [d3-graphviz](https://github.com/magjac/d3-graphviz) - Graphviz DOT rendering and animated transitions using D3.
* [smol](https://github.com/stjepang/smol) - small and fast async runtime for Rust.

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
