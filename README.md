<h1 align="center">
<img src="https://raw.githubusercontent.com/viatcheslavmogilevsky/flame/master/public/image/flame.png" alt="Flame Logo" title="Logo from Stockio (https://www.stockio.com)" />
<br>
flame
</h1>

## The core idea

Everything that can be containerized can be serverless.

Generic FaaS framework.

## How?

Provide preloaded runtime (process-pool or thread-pool) for wide range of tasks: online service, on-demand job, interactive shell (if possible), etc

## Prerequisites

1.  Application code itself, of course
2.  Make container image of application code
3.  Setup flame framework on container orchestration system (plain docker, Fargate, ECS, Kubernetes, etc)
4.  That's it!

