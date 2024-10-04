# Using Parquet files with Evidence

A short demo of how to use Parquet files with Evidence.

1. Create a new `DuckDB` connection, and use an in memory database, by calling the filename `:memory:`.
2. Put your parquet files in the **root** of the project (not in the source folder!)
3. Create a query to read the parquet file, and use the `read_parquet` function to read the file. `select * from read_parquet('filename.parquet').

See the example in `sources/needful_parquet`, which reads the parquet file `orders.parquet`.

