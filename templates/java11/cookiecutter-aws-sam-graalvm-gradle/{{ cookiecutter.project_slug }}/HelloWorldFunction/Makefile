.PHONY: build
build:
	cd .. && docker build -t al2-graalvm-gradle .

build-HelloWorldFunction:
	rm -rf ./build
	./gradlew clean
	./gradlew nativeCompile
	cp ./build/native/nativeCompile/native $(ARTIFACTS_DIR)
	cp ./build/resources/main/bootstrap $(ARTIFACTS_DIR)