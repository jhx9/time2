# time-tracker
Java (Maven) application for tracking time on the job

## Purpose

This purpose of this project is to show how to use Maven and Jenkins together.
 <reporting>
        <plugins>
            <plugin>
                <groupId>org.codehaus.mojo</groupId>
                <artifactId>findbugs-maven-plugin</artifactId>
                <version>3.0.1</version>
                <configuration>
                    <effort>Max</effort>
                    <threshold>Low</threshold>
                    <xmlOutput>true</xmlOutput>
                </configuration>
            </plugin>
            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-pmd-plugin</artifactId>
                <version>3.4</version>
                <reportSets>
                    <reportSet>
                        <reports>
                            <report>pmd</report>
                            <report>cpd</report>
                        </reports>
                    </reportSet>
                </reportSets>
            </plugin>
            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-checkstyle-plugin</artifactId>
                <version>2.15</version>
            </plugin>
        </plugins>
    </reporting>