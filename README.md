# Template AWS CDK Python Github Repository

A repository to use as a template for other aws cdk python repositories.

## Setup

### npm

npm is used to manage all node dependencies.

```shell
npm install
```

### pipenv

Pipenv is used to manage all python dependencies.

```shell
pip install pipenv
```

```shell
pipenv install -d
```

```shell
pipenv shell
```

### CDK

#### 1. Delete Placeholder Files

Delete the plcaeholde files found in 
[cdk/apps/sample_app/](/cdk/apps/sample_app/) and 
[cdk/bootstrap/](/cdk/bootstrap/).

#### 2. Rename Application

```sehll
# Change sample app to your applicat_ion name
mv cdk/apps/sample_app cdk/apps/{app_name}
```

#### 3. Initialse CDK App

The following will generate all the required files for a CDK python application,
though please note, that instead of utilising the generated virtual environment
created as part of the `cdk init`, I've opted to use a pipenv instead. The
generated virtual environment files can be discarded.

```sehll
cd cdk/apps/{app_name}
```

```shell
cdk init app --language python
```