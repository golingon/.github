# Lingon 🍒 - Libraries for building platforms with Go

## What is this?

Write [Terraform](https://github.com/golingon/lingon/tree/main/docs/terraform/) (HCL) and [Kubernetes](https://github.com/golingon/lingon/tree/main/docs/kubernetes/) (YAML) in Go. see [Rationale](https://github.com/golingon/lingon/tree/main/docs/rationale.md) for more details.

> Lingon is not a platform, it is a thin wrapper around terraform and kubernetes API in a library
> meant to be consumed in a Go application that platform engineers write to manage their platforms.
> It is a tool to build and automate the creation and the management of platforms regardless of the target infrastructure and services.

### It can do 4 things so far

- import kubernetes YAML manifests to valid Go code (even CRDs)  `kube.Import`
- export Go code to kubernetes YAML manifests  `kube.Export`
- generate Go code from Terraform providers `terragen.GenerateProviderSchema` and `terragen.GenerateGoCode`
- export terraform Go code to valid Terraform HCL  `terra.Export`

The only dependencies you need are:

- Go
- Terraform CLI
- kubectl

## Who is this for?

Lingon is aimed at advanced platform teams who need to automate the lifecycle of their cloud infrastructure
and have suffered the pain of configuration languages and complexity of gluing tools together with more tools.

## Project status

This project is in beta.
The APIs are stable, but we do not promise backward compatibility at this point.
We will eventually promise backward compatibility when the project is more battle tested.

This was a proof-of-concept at [volvo-cars](https://github.com/volvo-cars).
Unfortunately the project for which Lingon was being developed ended.
The original authors ([jacob](https://github.com/jlarfors) and [julien](https://github.com/veggiemonk)) believe in the concept and are
now maintainers of this project and will make sure it is healthy and receives updates.

See [FAQ](https://github.com/golingon/lingon/tree/main/docs/faq.md) for more details.

<!--

**Here are some ideas to get you started:**

🙋‍♀️ A short introduction - what is your organization all about?
🌈 Contribution guidelines - how can the community get involved?
👩‍💻 Useful resources - where can the community find your docs? Is there anything else the community should know?
🍿 Fun facts - what does your team eat for breakfast?
🧙 Remember, you can do mighty things with the power of [Markdown](https://docs.github.com/github/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
-->
