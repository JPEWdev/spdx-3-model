SPDX-License-Identifier: Community-Spec-1.0

# RelationshipType

## Summary

Information about the relationship between two Elements.

## Description

Provides information about the relationship between two Elements.
For example, you can represent a relationship between two different Files,
between a Package and a File, between two Packages, or between one SPDXDocument and another SPDXDocument.

Relationship names be descriptive enough to easily deduce the correct direction
from their name. The best way to do this is to make sure that the relationship
name completes the sentence:

`from` (is) (a) `RELATIONSHIP` `to`

## Metadata

- name: RelationshipType

## Entries

- affects: (Security/VEX) The `from` vulnerability affect each `to` Element
- amendedBy: The `from` Element is amended by each `to` Element
- hasAncestor: The `from` Element has ancestor described by each `to` Element
- availableFrom: The `from` Element is available from the additional supplier described by each `to` Element
- hasBuildDependencyOn: The `from` Element has a build dependency on each `to` Element
- usesBuildTool: The `from` Element uses each `to` Element as a build tool
- coordinatedBy: (Security) Used to identify the vendor, researcher, or consumer agent performing coordination for a vulnerability
- hasConcludedLicense: The `from` Software Artifact is concluded by the SPDX data creator to be governed by each `to` license
- contains: The `from` Element contains each `to` Element
- configOf: The `from` Element is a configuration applied to each `to` Element during a LifecycleScopeType period
- copiedTo: The `from` Element has been copied to each `to` Element
- hasDataFile: The `from` Element treats each `to` Element as a data file
- hasDeclaredLicense: The `from` Software Artifact was discovered to actually contain each `to` license, for example as detected by use of automated tooling.
- hasDependencyManifest: The `from` Element has manifest files that contain dependency information in each `to` Element
- dependsOn: The `from` Element depends on each `to` Element
- descendantOf: The `from` Element is a descendant of each `to` Element
- describes: The `from` Element describes each `to` Element. To denote the root(s) of a tree of elements in a collection, the rootElement property should be used.
- hasDevDependency: The `from` Element has a development dependency on each `to` Element
- hasDevTool: The `from` Element uses each `to` Element as a development tool
- hasDistributionArtifact: The `from` Element is distributed as an artifact in each Element `to`, (e.g. an RPM or archive file)
- hasDocumentation: The `from` Element is documented by each `to` Element
- doesNotAffect: (Security/VEX) The `from` Vulnerability has no impact on each `to` Element
- hasDynamicLink: The `from` Element dynamically links in each `to` Element
- hasExample: Every `to` Element is an example for the `from` Element (`from` hasExample `to`)
- hasEvidence: (Dataset) Every `to` Element is considered as evidence for the `from` Element (`from` hasEvidence `to`)
- expandsTo: The `from` archive expands out as an artifact described by each `to` Element
- exploitCreatedBy: (Security) Designates an agent has created an exploit against a vulnerability
- hasAddedFile: Every `to` Element is is a file added to the `from` Element (`from` hasAddedFile `to`)
- hasDeletedFile: Every `to` Element is a file deleted from the `from` Element (`from` hasDeletedFile `to`)
- modifiedBy: The `from` Element is modified by each `to` Element
- fixedBy: (Security) Designates a vulnerability has been fixed by an agent
- fixedIn: (Security/VEX) A vulnerability has been fixed in one or more elements
- foundBy: (Security) Designates an agent was the original discoverer of a security vulnerability
- generates: The `from` Element generates each `to` Element
- hasAssessmentFor: (Security) Relates a Vulnerability and an Element with a security assessment.
- hasAssociatedVulnerability: (Security) Used to associate a security vulnerability with a software artifact
- hasHost: The `from` Build was run on the `to` Element during a LifecycleScopeType period (e.g. The host that the build runs on)
- hasInputs: The `from` Build has each `to` Elements as an input during a LifecycleScopeType period.
- invokedBy: The `from` Build was invoked by the `to` Agent during a LifecycleScopeType period.
- hasMetafile: metafile: Every `to` Element is is a file containing metadata about the `from` Element (`from` hasMetafile `to`)
- delegatedTo: The `from` Agent is delegated to each `to` Agent during a LifecycleScopeType period, (e.g. `to` is acting on behalf of `from`)
- hasOptionalComponent: Every `to` Element is an optional component of the `from` Element (`from` hasOptionalComponent` `to`)
- hasOptionalDependency: Every `to` Element is an optional dependency of the `from` Element (`from` hasOptionalDependency` `to`)
- other: Every `to` Element is related to the `from` Element where the relationship type is not described by any of the SPDX relationhip types (this relationship is directionless)
- hasOutputs: The `from` Build element generates each `to` Element as an output during a LifecycleScopeType period.
- packagedBy: Every `to` Element is a packaged form of the `from` Element (`from` packagedBy `to`)
- patchedBy: Every `to` Element is a patch for the `from` Element (`from` patchedBy `to`)
- hasPrerequsite: The `from` Element has a prerequsite on each `to` Element
- hasProvidedDependency: The `from` Element has a dependency on each `to` Element, but dependency is not in the distributed artifact, but assumed to be provided
- publishedBy: (Security) Designates the agent that made a vulnerability record available for public use or reference
- reportedBy: (Security) Designates the agent that first reported a vulnerability to the project, vendor, or tracking database for formal identification
- republishedBy: (Security) Designates the agent that tracked, aggregated, and/or enriched vulnerability details to improve context (i.e. NVD)
- hasRequirement: The `from` Element has a requirement on each `to` Element
- hasRuntimeDependency: The `from` Element has a runtime dependency on each `to` Element
- serializedInArtifact: The `from` SPDXDocument can be found in a serialized form in each `to` Artifact
- hasSpecification: Every `to` Element is a specification for the `from` Element (`from` hasSpecification `to`)
- hasStaticLink: The `from` Element statically links in each `to` Element
- hasTest: Every `to` Element is a test artifact for the `from` Element (`from` hasTest `to`)
- hasTestCase: Every `to` Element is a test case for the `from` Element (`from` hasTestCase `to`)
- hasTestDependency: The `from` Element has a test dependency on each `to` Element
- hasTestTool: The `from` Element uses each `to` Element as a test tool
- testedOn: (AI, Dataset) The `from` Element has been tested on the `to` Element
- trainedOn: (AI, Dataset) The `from` Element has been trained by the `to` Element(s)
- underInvestigationFor: (Security/VEX) The impact of a vulnerability is being investigated
- hasVariant: Every `to` Element is a variant the `from` Element (`from` hasVariant `to`)
