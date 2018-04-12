<h1 align="center">
<img src="https://github.com/viatcheslavmogilevsky/flame/raw/master/public/images/flame.png" alt="Flame Logo" title="Logo from Stockio (https://www.stockio.com)" />
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

## Roadmap

### Fork'n'Go (one function call -> one process)


<table>
  <tr>
    <th></th>
    <th>plain docker</th>
    <th>Fargate</th>
    <th>ECS</th>
    <th>Kubernetes</th>
    <th>Other (mesos, CoreOS..,)</th>
  </tr>
  <tr>
    <td>Service</td>
    <td>❎</td> 
    <td>❎</td>
    <td>❎</td>
    <td>❎</td> 
    <td>❎</td>
  </tr>
  <tr>
    <td>Job</td>
    <td>❎ 📍</td> 
    <td>❎</td>
    <td>❎</td>
    <td>❎</td> 
    <td>❎</td>
  </tr>
  <tr>
    <td>Interactive</td>
    <td>❎</td> 
    <td>❎</td>
    <td>❎</td>
    <td>❎</td> 
    <td>❎</td>
  </tr>
</table>


### Spaw'n'Go (one function call -> one thread)

<table>
  <tr>
    <th></th>
    <th>plain docker</th>
    <th>Fargate</th>
    <th>ECS</th>
    <th>Kubernetes</th>
    <th>Other (mesos, CoreOS..,)</th>
  </tr>
  <tr>
    <td>Service</td>
    <td>❎</td> 
    <td>❎</td>
    <td>❎</td>
    <td>❎</td> 
    <td>❎</td>
  </tr>
  <tr>
    <td>Job</td>
    <td>❎</td> 
    <td>❎</td>
    <td>❎</td>
    <td>❎</td> 
    <td>❎</td>
  </tr>
  <tr>
    <td>Interactive</td>
    <td>❎</td> 
    <td>❎</td>
    <td>❎</td>
    <td>❎</td> 
    <td>❎</td>
  </tr>
</table>


