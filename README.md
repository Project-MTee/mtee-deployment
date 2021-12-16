## Project MTee platform configuration

This repository provides a minimal example of Kubernetes configuration to run the MTee platform. Configuration files are
only provided to illustrate how communication between components should be set up and is not suitable deployment as-is.

For more information, please refer to the more detailed
platform [documentation](https://github.com/Project-MTee/mtee-platform/wiki) and to the documentation of each component
separately. A working demo of this platform can be found at [here](https://mt.cs.ut.ee).

The MTee platform consists of the following dockerized components:

- Existing standard components
    - [RabbitMQ message broker](https://www.rabbitmq.com/)
    - [MySQL database](https://www.mysql.com/)
- Custom MTee components:
    - [Translation website](https://ghcr.io/project-mtee/website)
    - [Web translation proxy](https://ghcr.io/project-mtee/web-proxy)
    - [Translation API](https://ghcr.io/project-mtee/translation-api-service)
    - [Translation system service](https://ghcr.io/project-mtee/translation-system-service)
    - [Translation worker](https://ghcr.io/project-mtee/translation-model)
    - [Domain detection worker](https://ghcr.io/project-mtee/domain-detection-model)
    - [File translation service](https://ghcr.io/project-mtee/file-translation-service)
    - [File translation worker](https://ghcr.io/project-mtee/file-translation-worker)
- Integrated components:
    - [Grammatical error correction API](https://ghcr.io/tartunlp/grammar-api)
    - [Grammatical error correction worker](https://ghcr.io/tartunlp/grammar-worker)
    - [Automatic speech recognition API](https://ghcr.io/tartunlp/speech-to-text-api)
    - [Automatic speech recognition worker](https://ghcr.io/tartunlp/speech-to-text-worker)