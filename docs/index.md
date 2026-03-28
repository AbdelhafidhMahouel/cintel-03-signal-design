# Continuous Intelligence

This site provides documentation for this project.
Use the navigation to explore module-specific materials.

## How-To Guide

Many instructions are common to all our projects.

See
[⭐ **Workflow: Apply Example**](https://denisecase.github.io/pro-analytics-02/workflow-b-apply-example-project/)
to get these projects running on your machine.

## Project Documentation Pages (docs/)

- **Home** - this documentation landing page
- **Project Instructions** - instructions specific to this module
- **Your Files** - how to copy the example and create your version
- **Glossary** - project terms and concepts

## Additional Resources

- [Suggested Datasets](https://denisecase.github.io/pro-analytics-02/reference/datasets/cintel/)


## Custom Project

### Dataset
The dataset used in this project is a system metrics dataset that includes the number of requests, number of errors, and total latency in milliseconds. Each row represents one observation of system performance.

### Signals
I used the original signals from the example, including error rate, average latency, and throughput. I also created a new signal called `high_error_flag`, which is a binary indicator that becomes 1 when the error rate is greater than 5% and 0 otherwise.

### Experiments
I modified the pipeline by adding a new signal to detect high error conditions. I tested the pipeline after the modification to ensure it runs correctly and produces the expected output.

### Results
The output dataset included the new `high_error_flag` column along with the existing signals. This made it easier to identify rows where the system experienced high error rates.

### Interpretation
This modification helps improve system monitoring by making it easier to detect abnormal behavior. Instead of only looking at raw error rates, the binary flag highlights critical situations quickly. This can help support faster decision-making and improve system reliability.
