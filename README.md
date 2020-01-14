# eis-manifests

This repo hosts the manifest files needed to demonstrate multiple usecases in Edge Insights Software

# Using repo tool

1. Fetching the manifests from eis-manifests repo:
    ```
    repo init -u "ssh://git@gitlab.devtools.intel.com:29418/Indu/IEdgeInsights/eis-manifests"
    ```

2. Providing your own manifest:
    * Have the manifest file added in ".repo/manifests/" directory from where you want to clone all the repos and run the below command:
      ```
      repo init -m <manifest_file.xml>
      ```

3. Run the below command to clone all the repos mentioned in the manifest:
    ```
    repo sync
    ```

4. To fetch manifests from a URL which is not merged to master and pushed to a certain branch, run the below command:
    ```
    repo init -u <path_to_manifests_repo> -b <branch_name>
    ```
