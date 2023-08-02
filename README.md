# rafa-astro-repo-example-two
This is a mono repo for multiple Astro deployments


# CI/CD process

```mermaid
graph LR;
    subgraph team
        astro-dir
    end
    subgraph ci-cd
        team/astro-dir
    end
    subgraph astro
        deployment
    end
    
    astro-dir-->ci-cd;
    ci-cd->deployment;
```