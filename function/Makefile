build-JavaFunction:
	mkdir -p "$(ARTIFACTS_DIR)/lib"
	mvn clean package
	mvn dependency:copy-dependencies -DexcludeScope=provided
	cp -rf ./target/*.jar "$(ARTIFACTS_DIR)/lib/"
	rm -rf ./target