Apps-library
============
# [HFactory](http://hfactory.io)

HFactory is a Scala-based micro-framework to simplify and speed up the development of HBase powered web applications. This github repository contains open-source applications, samples and utilities complementing the HFactory platform.

## Table of contents

- <a href="#prerequisites">Prerequisites</a>
- <a href="#getting-started">Getting started</a>
- <a href="#contributing">Contributing</a>
- <a href="#documentation">Documentation</a>
- <a href="#support">Support</a>

## <a href="#prerequisites" id="prerequisites">Prerequisites</a>

To run applications, an HFactory Server is needed. A fully-featured version can be downloaded free of charge and without prior registration from [hfactory.io](http://hfactory.io/download.html#server). For production use (defined as working on a dataset of more than 100k HBase cells), you will need a production license from [Ubeeko](http://ubeeko.com).

## <a href="#getting-started" id="getting-started">Getting started</a>

#### Start your HFactory Server

- Download the HFactory Server archive from [hfactory.io](http://hfactory.io/download.html).
- Install the server by unzipping the HFactory Server archive in the /usr/local directory or one of your choosing and modify the server's configuration file accordingly (in particular, the app store path and the license path).
- Choose the HBase configuration file to use by setting hserver.hbase.conf, and make it to point to your HBase instance. Base platform-specific configurations are provided in the HFactory Server archive:
-- hbase-site.properties for Cloudera or Apache;
-- hbase-site.properties.hortonworks for Hortonworks;
-- hbase-site.properties.mapr for MapR.
- Start the server with /usr/local/hfactory-server/bin/start-server.sh.

Troubleshooting: If the server fails to start because Java is not found, set environment variable JAVA_HOME to the location of the Java runtime before starting the server.

#### List of available open-source applications

| Application | Description                                                      | source                                        | build                                       |
| ----------- | ---------------------------------------------------------------- | --------------------------------------------- | ------------------------------------------- |
| Hotspot     | HBase web app using composite rowkeys for geographic coordinates | [github](https://github.com/hfactory/Hotspot) | [zip](http://hfactory.io/assets/Hotspot.zip |

#### Launch open-source apps

- Copy or unzip the application folder exported from the studio in /usr/local/hfactory-server/apps (or in your custom app store path)
- Go to the server administration page http://localhost:18090 by default
- Create the tables if needed
- Start the application
- Click the application name once it is started

More information in the [documentation](#documentation)

#### Build your own custom apps

To modify showcase apps or create your own ones, best is to use [HFactory Studio](http://hfactory.io/download.html#studio), the free, fully-packaged IDE tailored for the HFactory platform. Just place the github project in the workspace folder and import it with eclipse. And then it's up to you, you can obviously keep your apps in-house or decide to <a href="#contributing">share</a> part or all of them with the community.

## <a href="#contributing" id="contributing">Contributing</a>

This project welcomes new contributors. If you would like to help make HFactory better by adding new applications, enhancing existing applications, or fixing bugs, we will be glad to have you work alongside us.

Submissions on this repository are made pursuant the terms of the Apache License, Version 2.0 (http://www.apache.org/licenses/LICENSE-2.0.html) and constitute "Contributions," as defined therein, and you represent and warrant that you have the right and authority to do so.

When adding new files, please include the following Apache v2.0 license header at the top of the file, with the fields enclosed by brackets "[]" replaced with your own identifying information. (Don't include the brackets!):
<pre><code>
/*
 * Copyright (c) [XXXX] [NAME OF COPYRIGHT OWNER]
 *
 * Licensed under the Apache License, Version 2.0 (the "License");
 * you may not use this file except in compliance with the License.
 * You may obtain a copy of the License at
 *
 *   http://www.apache.org/licenses/LICENSE-2.0
 *
 * Unless required by applicable law or agreed to in writing, software
 * distributed under the License is distributed on an "AS IS" BASIS,
 * WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 * See the License for the specific language governing permissions and
 * limitations under the License.
 */
 </code></pre>
 Thanks a lot for contributing!

## <a href="#documentation" id="documentation">Documentation</a>

 The complete HFactory documentation is available on the project community web site [hfactory.io](http://hfactory.io).

## <a href="#support" id="support">Support</a>

Please use the HFactory discussion group for open, public support. Subscription to the group is open and postings are welcome. You can signup by going to the following url [https://groups.google.com/forum/#!forum/hfactory](https://groups.google.com/forum/#!forum/hfactory)
