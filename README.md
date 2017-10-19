# ironmegalodon

Google Cloud Dataflowを利用して、全文検索用のIndexを作成する

```
mvn compile exec:java -Dexec.mainClass=org.sinmetal.beam.ironmegalodon.Ironmegalodon -Dexec.args="--runner=DataflowRunner --project=sinmetal-dataflow \
     --tempLocation=gs://staging.souzoh-p-sinmetal.appspot.com/tmp" -Pdataflow-runner
```