# LUME Prefect Orchestration Demo

The notebooks in this repo are part of a demonstration on how to orchestrate LUME simulations using [Prefect.io](https://prefect.io/).

## Dependencies

- Python >=3.7
- prefect
- lume-base
- lume-astra
- lume-impact
- distgen

# Notebooks

## lume-flow

This notebook demonstrate how to create tasks and flows using Prefect.

The first demonstration uses a local agent and runs the tasks in a sequence.

The second demonstration uses a local Dask agent and runs the independent tasks in parallel without changes to the Flow.

The last demonstration on this notebook covers how to retrieve the objects back from the Flow State and tasks.

## lume-flow-server

This notebook demonstrate how to leverage a Prefect Local Server and the Prefect UI.

### Starting the Local Server

```bash
prefect server start
```

### Starting the Local Agent

```bash
prefect agent local start
```

### Creating a Project

```bash
prefect create project "lume-orchestration"
```