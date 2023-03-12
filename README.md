# Carrot Market

Serverless Carrot Market Clone using NextJS, Tailwind, Prisma, PlanetScale and Cloudflare.

## PlanetScale environment set up
[link](https://planetscale.com/docs/concepts/planetscale-environment-setup)
### Windows instructions
On Windows, pscale is available via [scoop](https://scoop.sh/), and as a downloadable binary from the [releases](https://github.com/planetscale/cli/releases/latest) page:
Open a PowerShell terminal (version 5.1 or later) and run:
```
> Set-ExecutionPolicy RemoteSigned -Scope CurrentUser # Optional: Needed to run a remote script the first time
> irm get.scoop.sh | iex
```
```
scoop bucket add pscale https://github.com/planetscale/scoop-bucket.git
scoop install pscale mysql
```
```
pscale auth login
pscale region list
pscale database create carrot-market --region ap-northeast
pscale connect carrot-market
```