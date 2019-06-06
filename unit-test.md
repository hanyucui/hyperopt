Running unit tests
==============

To run the  unit tests, run the `run-tests.sh` script.  You will need to set these environment variables:

- `SPARK_HOME`: your local copy of Apache Spark. Look at download_spark_dependencies.sh for more details.
- `HYPEROPT_FMIN_SEED`: the random seed. You need to get its value from `.travis.yml`.

For example:

```bash
hyperopt$ HYPEROPT_FMIN_SEED=3 SPARK_HOME=/usr/local/lib/spark-2.4.0-bin-hadoop2.7 ./run_tests.sh
```

To run the unit test for one file, you can add the file name as the parameter, e.g:
```bash
hyperopt$ HYPEROPT_FMIN_SEED=3 SPARK_HOME=/usr/local/lib/spark-2.4.0-bin-hadoop2.7 ./run_tests.sh hyperopt/tests/test_spark.py
```
