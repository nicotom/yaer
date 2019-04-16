#  YAER (Yet Another Experiment Runner)
Tool to run experiments

## Usage
Usage: yaer [OPTIONS] COMMAND [ARGS]...

Options:
  --verbose  Enable debug logging.
  --version  Show the version and exit.
  --help     Show this message and exit.

Commands:
  list  List available experiments.
  run   Run listed experiments with provided datasets.

Arguments:
RUN
-e, --experiment            Experiment to run. This can be specified multiple times. See list command por options.
-d, --dump                  Dump results and files.
--clean-previous-results    Remove previous results for every executed experiment.
--dump_path                 Base path to dump results and files.

## Examples
```bash
# List available experiments
./tools/run.sh list
```

```bash
# Run defined experiments
./tools/run.sh --verbose run -e experiment1 -e experiment2 -d
```
