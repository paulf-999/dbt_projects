# Python Scripts

The python files used in this repo are largely used in combination with Jinja templates to generate files required for every dbt project.

* `py/gen_dbt_src_properties.py` - this script is used to generate the dbt `_source.yml` resource properties file using Jinja templates within the directory `templates/src_properties_generator/`.
* `py/gen_dbt_sql_objs.py` - this script is used to generate dbt snapshot or incremental sql files in bulk, using the Jinja templates `templates/snapshot.sql.j2` and `templates/incremental.sql.j2`.
* `py/gen_dbt_model_directory.py` - this script is used to recreate the [target dbt project structure recommended by dbt](https://docs.getdbt.com/guides/best-practices/how-we-structure/1-guide-overview#guide-structure-overview).

For more information on the Jinja templates used by each of the Python scripts above, see: [`templates/README.md`](templates/README.md).