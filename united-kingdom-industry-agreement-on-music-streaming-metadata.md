# Background
In the era of digital music, good quality metadata, which describes who contributed to a track’s creation and how, is essential to making sure music makers are accurately credited and paid. But metadata is often not as accurate or complete as it should be, in particular in relation to songwriters and their works. Incomplete or inaccurate metadata can lead to significant delays to creators being paid for the use of their works, and in some cases not being paid at all.

Experts from across the UK music industry have come together to take positive steps to improve music metadata, for the benefit of all. Whilst many aspects of metadata provision work well, and positive steps to improve it are being taken in many parts of the industry, key challenges remain in a number of areas. This includes sourcing metadata from creators in a timely manner and the adoption of and access to standard industry identifiers, especially in relation to work and songwriter metadata. In particular, the link between sound recording and musical work metadata and which party is the authoritative source of this link is a key challenge.

This document sets out a roadmap for how industry and Government will work together to deliver consistent high quality metadata, supported by best practice, education and well-functioning systems.

## Ambition and Approach
The signatories agree that music metadata should be complete, authoritative, and available to those who need it when they need it, enabling contributors to works and recordings to be credited and paid accurately and promptly.

In relation to work and songwriter metadata the signatories agree to the following:

**During the course of two years** from the publication of this agreement, to collaborate and progressively improve the quality and timeliness of work and songwriter metadata associated with new recordings on streaming services so that:

- complete work and songwriter data, including identifiers where available, is provided to streaming services in similar timeframes as recording and artist metadata;
- works and songwriters are consistently credited on streaming services and identified in relevant reports to -licensors, including with identifiers, where available

To achieve this goal, they agree to:

- take steps to ensure a **core data set** is associated with all new recordings on streaming services (see below)
- follow and promote **good practice** (see Annex A below) , and;
- establish expert groups on **education** and **technical solutions** to drive forward concrete improvements in these areas during the two-year period (see Annex B below). The **education expert group** will develop and promote accessible educational resources, tailored to different audiences, to raise awareness of the importance of metadata. - The **technical solutions expert group** will explore current workflows, standards and technologies and how to improve them to enable delivery of the core data set.

# Core Data Set
- A core data set should routinely and accurately be provided to streaming services with a recording. The core data set should comprise the following elements:
```
{
  "SoundRecordingMetadata": {
    "RecordingTitle": "Example Title",
    "Subtitle": "Example Subtitle",
    "RecordingArtists": [
      {
        "Name": "Artist Name",
        "IPN": "Artist's IPN if available",
        "ISNI": "Artist's ISNI if available"
      }
    ],
    "PerformerStudio": "Example Studio",
    "ProducerPersonnel": [
      {
        "Name": "Producer Name",
        "Role": "Producer",
        "IPN": "Producer's IPN if available",
        "ISNI": "Producer's ISNI if available"
      }
    ],
    "ISRC": "International Standard Recording Code"
  },
  "MusicalWorkMetadata": {
    "WorkTitle": "Example Work Title",
    "Subtitle": "Example Work Subtitle",
    "Writers": [
      {
        "Name": "Writer Name",
        "Role": "Composer",
        "IPI": "Writer's IPI if available",
        "ISNI": "Writer's ISNI if available"
      }
    ],
    "ISWC": "International Standard Musical Work Code"
  }
}
```

![image](https://github.com/JonathanBowker/music-streaming-metadata/assets/1875500/7f568bf0-ad79-4e02-a4a6-6cb6a6123b06)

## Adoption of the Core Data Set
The above elements represent the core data set that should accompany tracks which are available on streaming services, allowing contributors to be credited and paid more quickly and accurately. The aim is to make significant improvements in provision of this data set over the two-year period.

It is already within the capability of many players in the streaming value chain to provide much of this data set, for example work and recording titles and writer and artist names. There is a strong expectation that signatories to this agreement provide this data, where reasonably available to them, and commit to implement, maintain, and update systems and processes to support this.

The IPI and ISWC are the preferred identifiers for songwriters and works. Although these identifiers are recognised as the best way to ensure accurate identification of writers and works, they are not used throughout the industry, and there are often challenges in obtaining them. In order to achieve wider adoption, the signatories agree to work together and with international partners including CISAC to make these identifiers more readily available to those who need them. Should sufficient progress on making IPI and ISWC more easily available not be made early on during the period covered by this agreement, alternatives may need to be considered.

The signatories also recognise the importance of ISNI, both as an alternative to the IPI and to describe other contributors to recordings.

## Measuring implementation
The technical solutions expert group will be tasked with developing Key Performance Indicators (KPIs) to measure the implementation of the core data set. This should include metrics relating to the provision of the core data set at the point of upload and the use of the core data set in relevant reports to licensors. This should be one of the first tasks of the technical solutions expert group and should be completed within the first six months following publication of this agreement.

When developing metrics, the group should assess the baseline position of different data elements, and consider variations in the creative process (e.g. covers, medleys, samples etc.) to determine what significant but achievable progress will look like in relation to each element at the end of the two-year period covered by this agreement. This should in particular take into account challenges in relation to providing the IPI and ISWC versus other data elements.

## Beyond the two-year period
At the end of the two-year period covered by this agreement, the aim is that significant progress will have been made in provision of the core data set. Building on this progress, the signatories will consider how to achieve higher standards of provision beyond the two-year period.

# Oversight
The goals, best practice and deliverables set out above will be implemented over the course of two years. To support this, the following system of oversight will be put in place.

1. **The Intellectual Property Office (IPO**) will play an ongoing role as supervisor and facilitator. It will facilitate and monitor implementation of this agreement, ensure progress is reported, and attempt to broker a resolution to any issues which arise. It will provide formal updates to government ministers and industry representatives.
2.** A Steering Group** will be established to guide and support implementation. This group will be chaired by the IPO and comprise industry representatives selected by them, who are broadly representative of the signatories to the agreement. It will receive reports from the expert groups and support the implementation of commitments. Members will be responsible individually and collectively for driving progress to fulfil the commitments The Steering Group will meet formally every 6 months, with email correspondence and ad-hoc meetings as required.
3. **Expert Working Groups** on education and technical solutions will be established to work towards the goals described above. These will comprise relevant experts with deep expertise in their areas of delivery. They will provide regular updates to the Steering Group, which will monitor their progress and provide support and guidance.

# Annex A: Code of Good Practice
The signatories to the Agreement agree to implement, follow and promote good practice standards in the use of music metadata.

The signatories agree that good practice includes, but is not limited to, the following:

1. **Songwriters** should record and provide accurate information relating to their copyright works as close as possible to the point of creation. This should include their full given names and respective roles and, where available, identifiers and rights ownership information.
2. **Recording Artists** should record and provide accurate information relating to their performances at the point of recording. This should include their respective roles and IPN and/or ISNI numbers, where available.
3. **Artist Managers** should take all reasonable steps to obtain the core data described above for artists and songwriters they represent and provide to releasing parties and publishers in a timely manner.
4. **Artist Managers and Publishers** should ensure that songwriters agree their respective contributions and song splits on new works as early as possible.
5. **Studio producers** should seek to provide the core data set for each recording to the releasing party with the recording itself.
6. **Studio producers, artist managers and label and publisher** A&R should cooperate and make best efforts to assemble and provide core data to releasing parties, as appropriate to their individual roles and the circumstances of a given release.
7. **Publishers and CMOs** should promote the ISWC and IPI as the standard identifiers for musical works and songwriters and work with CISAC and others to make these identifiers easier to issue, access and use by a wide range of parties.
8. **Publishers should**:
- use the new CISAC ISWC assignment system to enable early assignment via their CMO/SPV
- register their works with CMOs/SPVs before or as close as possible to a recording release date (subject to timely and accurate provision of upstream data from creators and managers)
- ensure that registrations are as complete as possible including all core work metadata and any known recording metadata before or as close as possible to a recording release date
- allow their work identifier data to flow into current and future good practice data flows either directly or via their chosen society
- ingest enrichments passed back by CMOs/SPVs, including ISWCs, ISRCs, and include them in any subsequent registrations and deliveries to third parties
9. **CMOs should**:
- improve speed and automation of work registration to enable ISWC to be issued and made available before or as close as possible to a recording release date (subject to timely provision of upstream data by creators, managers, and publishers)
- pass all relevant enrichments (e.g. ISWCs, IPIs, matched ISRCs, etc.) back to publishers and to service providers via appropriate channels, such as the musical work claims process
10. **Releasing parties should**:
- capture all core recording data for which they are authoritative (Recording Title and Sub-title, Recording Artist, ISRCs, names, roles and identifiers where available for performers and studio personnel)
- pass on to service providers all accurate core metadata that has been made available to them in relation to a track, including any work, songwriter and performer information and identifiers, and actively encourage provision of such metadata by suppliers
- ensure that core metadata fields are available to users of distributors and other services to enable this data to be captured and passed on as required
- ensure that labels’ contracts with studio producers include a clause to ensure that all contributors to recordings are asked to identify themselves, including with IPI/IPN codes where possible, and all available core data, including IPI and ISWC where available, is delivered to the releasing party
11. **Service providers should**:
- ingest all core metadata provided to them by releasing parties to enable accurate identification of works and recordings
- explore and develop methods to incentivise the complete inclusion of the core data set, including through engagement with the technical solutions expert group;
- ensure that provided credits are accurately displayed, and visible to consumers on their services, where reasonable and in accordance with agreed industry guidelines; and endeavour to make credits searchable
- report, materially unchanged or changed where reasonable and in accordance with agreed industry guidelines, all core metadata that they hold to relevant rightsholders that they have contracted with in an accurate and timely manner

## Implementation and further development
The practice set out above is intended to represent current good practice in the industry. Signatories should aim to implement this good practice as soon as they are able to. It should be noted that the good practice is not exhaustive and does not describe every use case where metadata is involved. As a result of ongoing developments in good practice, including through the work of the Expert Groups, it may be appropriate for the Code to be updated. For example, the Code may be updated to reflect improved processes and workflows, and new authoritative data sources. Any amendments to the Code would require agreement of the Steering Group, and endorsement by its signatories.

### Terminology
**Releasing parties** are those parties responsible for delivering the recording to service providers. This includes record labels, distributors and aggregators.

**Service providers** are providers of online music streaming services to consumers. For the purposes of this agreement, this does not include User Generated Content platforms.

**Collective Management Organisations (CMOs)** are licensing bodies which grant rights on behalf of multiple rights holders in a single blanket licence for a single payment and collect any royalties owed to the rights holders. CMOs and publishers may enact their obligations, where appropriate, via Special Purpose Vehicles (SPVs), which are joint ventures established by CMOs to license the repertoire of publishers and other rights holders.

A **work** is a musical or lyrical work – i.e. a song or composition.

A **recording** is a sound recording – i.e. a musical work that is recorded creates a sound recording.

A **track** contains both a musical work and a sound recording.

**International Standard Recording Code (ISRC)** – is a code which is used to identify sound recordings.

**International Standard Musical Work Code (ISWC)** – is a code which is used to identify a song or composition.

**International Performer Number (IPN)** is a code to identify a performer and is used in data exchanges between CMOs.

**Interested Party Information (IPI)** number is code which is assigned to songwriters, composers and music publishers by Performing Rights Organisations. These are attached to ISWC numbers to include information about authorship to works with an ISWC.

**International Standard Name Identifier (ISNI)** is used to identify persons including persona stage names and organisations involved in creative activities such as record labels.

# Annex B: Expert Working Groups
Expert groups will be established and mandated to develop, support and champion practical measures which enable increasing application of the core data set during the two-year period, building towards the future ambition and beyond.

This section sets out the remit and objectives for the expert groups and identifies possible areas of work and outputs. The groups themselves will develop detailed work plans, in order to meet their objectives. Membership of the groups will be limited to those with the right expertise who are best placed to develop solutions.

## Education Expert Group
Education and awareness of the importance of metadata is vital for all parts of the creative value chain, from those creating songs and recordings, through to those responsible for delivering data to platforms, CMOs and others, including artist managers and A&R departments. Consistent delivery of the core data set envisaged by this agreement will require high levels of awareness of the importance of metadata by creators and others. Membership of this group should comprise those with a good understanding of the needs of creators and other target audiences, educators and those skilled in effective communication, as well as data experts. Areas covered by this working group should include:

- mapping existing education resources across the industry and how to maximise access to these resources including DIY artists
- collating existing information on relevant systems and initiatives such as DDEX standards
- bringing together viewpoints from across the streaming ecosystem
- developing new appropriate and accessible educational resources, tailored to different audiences such as artists, songwriters, managers and A&R departments, to raise awareness of the importance of metadata
- considering how to best effectively raise awareness and standards of metadata input across the music industry at all levels with a communication strategy to maximise impact
- working with Credits Due and WIPO for Creators to maximise global reach

## Technical Solutions Expert Group
Industry acknowledges that well-functioning technology, supported by consistent standards, formats and rules, is fundamental to meeting the future metadata ambition. This group will consider current workflows, data authority, standards, formats and technologies, and how to improve them to support the consistent delivery of the core data set. The Metadata Code of Good Practice (Annex A) should be updated as appropriate should improved flows or new authoritative data sources be developed. Membership of this group will comprise experts who work with and control data systems and processes and are able to develop and deliver any required changes. The group will also seek close cooperation with international partners including DDEX and CISAC, to help support the development of international standards and encourage the wider availability of IPI and ISWC codes.

The IPO is committed to long term solutions and will fund an external consultant with music industry metadata knowledge to support the group. They will support the group to catalogue and map existing metadata flows and baseline and identify meaningful KPIs to be measured at key points in the data chain. The KPIs will be developed within six months of the project start date. They should be shared with the signatories to the agreement as soon as possible and published as appropriate.

Other outputs from the group should include:

- specifying easier and more transparent access to identifier codes and databases for more parties in the value chain, including publishers, labels, studios and DIY artists. It has been proposed that a plan should be developed to further open both scalable and individual creator access to necessary identifiers (IPI and ISWC) and associated databases to allow timely allocation over the two-year period
- exploring systems and processes for recording and sharing authoritative and definitive links between songs and recordings. This could mean developing new or enhanced data flows, building on existing databases or developing new ones, and could lead to a definitive ISRC-ISWC link registry. Any such systems or processes should be practical to implement and databases should be as open as possible and easily accessible to those who need to use them
- exploring systems, tools and processes to make it easier for creators and managers to capture and communicate metadata to others in the value chain. This could mean developing new tools, workflows and formats, or building on existing ones, that are easy to use and widely accepted across the value chain. It should also consider, with the education group, how to promote the uptake and adoption of data capture tools
- exploring enrichments to Service Provider Preferred Music Distributor Provider Programs
