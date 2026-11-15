
# Understanding PKI and Digital Certificates

## What I Learned

Public Key Infrastructure (PKI) is a framework for managing
digital certificates and cryptographic keys. It helps systems
establish trust.

## The Certificate Chain

1. **Root CA:** The top-level certificate authority.
   Its trusted certificate acts as a trust anchor.
2. **Intermediate CA:** A certificate authority authorized
   by a higher CA to issue certificates.
3. **Server certificate:** Binds a website's identity
   to its public key.

## How a Certificate Is Created

1. A server generates a public/private key pair.
2. The administrator creates a **CSR (Certificate Signing
   Request)** containing the public key and identifying information.
3. The CSR is submitted to a Certificate Authority.
4. The CA validates the request and issues a signed certificate.
5. The certificate is installed on the server.

**Important:** The private key is not included in the CSR.

## Real-World Example

When I visit an HTTPS website, my browser checks whether the
server certificate is valid and chains to a trusted root certificate.

## What Initially Confused Me

The Certification Authority vs the Registration Authority

## My Key Takeaway

A certificate is not automatically trustworthy simply because it
exists. The browser must validate its identity, validity
and chain of trust.

Important inforgraph:

