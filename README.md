# SmartHealth
Healthcare data using synthea simulated patient records

# Build Synthetic Patient Data


* run.sh

synthea/run_synthea -c /Users/tspann/Desktop/apps/synthea/run.settings -p 10000 "New Jersey"

* run.settings

exporter.ccda.export = true
exporter.fhir.export = true
exporter.hospital.fhir.export = true
exporter.fhir_stu3.export = false
exporter.fhir_dstu2.export = false
exporter.text.export = true
exporter.csv.export = true
exporter.csv.append_mode = true
exporter.years_of_history = 0

# example run

9986 -- Dinah304 MacGyver246 (63 y/o F) Jersey City, New Jersey 
9951 -- Lizabeth515 Schroeder447 (104 y/o F) Belleville, New Jersey 
Records: total=11958, alive=10000, dead=1958

BUILD SUCCESSFUL in 26m 57s
4 actionable tasks: 4 executed


# Resources

* https://github.com/synthetichealth/synthea
* https://github.com/FirelyTeam/fhirstarters/tree/master/java/hapi-fhirstarters-simple-server/
* https://hapifhir.io/hapi-fhir/docs/tools/hapi_fhir_cli.html
