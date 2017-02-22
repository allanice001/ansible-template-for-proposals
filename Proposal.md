# The Ansible Proposal process

The Core committee is responsible for evolving Ansible (the language), and authoring the specification. The committee operates by consensus and has discretion to alter the specification as it sees fit. However, the general process for making changes to the specification is as follows:

## Development
Changes to the language are developed by way of a process which provides guidelines for evolving an addition from an idea to a fully specified feature, complete with acceptance tests and multiple implementations. There are four "maturity" stages. The Core committee must approve acceptance for each stage.

<table>
  <caption>Maturity Stages</caption>
  <thead>
    <tr>
      <th>
      <th>Stage
      <th>Purpose
      <th>Entrance Criteria
      <th>Acceptance Signifies
      <th>Spec Quality
      <th>Post-Acceptance Changes Expected
      <th>Implementation Types Expected*
    </tr>
  </thead>
  <tr>
    <td>0
    <td>BrainDump vs LightBulb
    <td>Allow input into the specification
    <td>We'd like to see an issue created in our proposals repo
    <td>N/A
    <td>N/A
    <td>N/A
    <td>N/A
  </tr>
  <tr>
    <td>1
    <td>Proposal
    <td>
      <ul>
        <li>Make the case for the addition
        <li>Describe the shape of a solution
        <li>Identify potential challenges
      </ul>
    </td>
    <td>
      <ul>
        <li>Identified “champion” who will advance the addition
        <li>Prose outlining the problem or need and the general shape of a solution
        <li>Illustrative examples of usage
        <li>High-level API
        <li>Discussion of key algorithms, abstractions and semantics
        <li>Identification of potential “cross-cutting” concerns and implementation challenges/complexity
      </ul>
    </td>
    <td>The committee expects to devote time to examining the problem space, solutions and cross-cutting concerns
    </td>
    <td>None
    <td>Major
    <td>Polyfills / demos
  </tr>
  <tr>
    <td>2
    <td>Draft
    <td>Describe the syntax and semantics using formal spec language
    <td>
      <ul>
        <li>Above
        <li>Initial spec text
      </ul>
    </td>
    <td>The committee expects the feature to be developed and eventually included in the standard
    <td>Draft: all <em>major</em> semantics, syntax and API are covered, but TODOs, placeholders and editorial issues are expected
    <td>Incremental
    <td>Experimental
  </tr>
  <tr>
    <td>3
    <td>Candidate
    <td>Indicate that further refinement will require feedback from implementations and users
    <td>
      <ul>
        <li>Above
        <li>Complete spec text
        <li>Designated reviewers have accepted the current proposal text
        <li>The Core committee have accepted the current proposal text
      </ul>
    </td>
    <td>The solution is complete and no further work is possible without implementation experience, significant usage and external feedback.
    <td>Complete: all semantics, syntax and API are completed described
    <td>Limited: only those deemed critical based on implementation experience
    <td>Spec compliant
  </tr>
  <tr>
    <td>4
    <td>Finished
    <td>Indicate that the addition is ready for inclusion in the formal ECMAScript standard
    <td>
      <ul>
        <li>Above
        <li>Acceptance tests have been written for mainline usage scenarios, and merged
        <li>Two compatible implementations which pass the acceptance tests
        <li>Significant in-the-field experience with shipping implementations, such as that provided by two independent VMs
        <li>A pull request has been sent to <a href="https://github.com/ansible/ansible">ansible/ansible</a> with the integration
        <li>The Ansible core team have sight of the pull request, by it being added to a core meeting
        <li> The Identified “champion” or one of the community member should attend the core meenting where pull request is discussed.
      </ul>
    </td>
    <td>The addition will be included in the soonest practical standard revision
    <td>Final: All changes as a result of implementation experience are integrated
    <td>None
    <td>Shipping
  </tr>
</table>
