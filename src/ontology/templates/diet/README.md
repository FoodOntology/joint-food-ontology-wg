Google Sheet for Dietary terms: https://docs.google.com/spreadsheets/d/18Ml5pLHfd0IVGD3roxF0NkjXRry0rRrsa8Y06y2fgr0/edit#gid=0

Robot tool: http://robot.obolibrary.org

Robot template command: http://robot.obolibrary.org/template

robot template --template diet.tsv \
  --input ""obi_import.owl"" \
  --prefix ""TERM:http://purl.obolibrary.org/obo/TERM_"" \
  --prefix ""RO:http://purl.obolibrary.org/obo/RO_"" \
  --prefix ""oboInOwl:http://www.geneontology.org/formats/oboInOwl#"" \
  --prefix ""schema:http://schema.org/"" \
  --ontology-iri ""http://purl.obolibrary.org/foodon/imports/diet.owl"" \
  --output diet.owl"

as single line:
robot template --template diet.tsv --input "obi_import.owl" --prefix "TERM:http://purl.obolibrary.org/obo/TERM_"  --prefix "oboInOwl:http://www.geneontology.org/formats/oboInOwl#" --prefix "schema:http://schema.org/" --ontology-iri "http://purl.obolibrary.org/foodon/imports/diet.owl" --output diet.owl

