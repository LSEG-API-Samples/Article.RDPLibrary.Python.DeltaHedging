# Delta Hedging - Simplify your Option Pricing


## Table of Content

* [Overview](#overview)

* [Disclaimer](#disclaimer)

* [Prerequisites](#prerequisites)

* [Setup](#setup)


## <a id="overview"></a>Overview
In this example, I will present different workflows used to manage risk, specifically focusing on the most widely used Greek (Delta), as a tool to hedge common strategies.

Details and concepts are further explained in the [Delta Hedging - Simplify your Option Pricing](https://developers.refinitiv.com/article/delta-hedging-simplify-your-option-pricing) article published on the [Refinitiv Developer Community portal](https://developers.refinitiv.com).

## <a id="disclaimer"></a>Disclaimer
The source code presented in this project has been written by Refinitiv only for the purpose of illustrating the concepts of creating the "what-if" scenarios using the Refinitiv Data Platform Library for Python.  It has not been tested for usage in production environments.

***Note:** To [ask questions](https://community.developers.refinitiv.com/index.html) and benefit from the learning material, I recommend you to register on the [Refinitiv Developer Community](https://developers.refinitiv.com)*

## <a name="prerequisites"></a>Prerequisites

Software components used:

- [Refinitiv Data Platform](https://developers.refinitiv.com/refinitiv-data-platform/refinitiv-data-platform-apis): Access to the [pricing endpoint](https://api.refinitiv.com/) data services
- Python Environment:
  - Tested with Python 3.7
  - Packages: [rdp](https://pypi.org/project/refinitiv-dataplatform/) [pandas](https://pypi.org/project/pandas/) json datetime math dateutil enum
  - RDP for Python installation:  '**pip install refinitiv-dataplatform**'

## <a name="setup"></a>Setup

The application package includes the following:
* **DeltaHedging.ipynb**
  
  The Jupiter Notebook document represents the example containing the core Python instructions to execute our application.

  * **Platform Access**
    
    The Notebook includes the following code snippet to register your credentials to access the content.  
    
    **Note**: Access credentials to Pricing and Analytics data services are required.
    
    ```python
    rdp.open_platform_session(
      "<YOUR APP KEY>",
        rdp.GrantPassword(
          username = "<YOUR MACHINE ID>",
            password = "<PASSWORD>"
        )
    )
    ```

## Running the application

The application is executed within the `Jupyter notebooks` web-based environment.  Prior to running the application, ensure you have supplied your access credentials - refer to the Setup section above.

### <a id="contributing"></a>Contributing

Please read [CONTRIBUTING.md](https://gist.github.com/PurpleBooth/b24679402957c63ec426) for details on our code of conduct, and the process for submitting pull requests to us.

### <a id="authors"></a>Authors

* **Nick Zincone** - Release 1.0.  *Initial version*

### <a id="license"></a>License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

