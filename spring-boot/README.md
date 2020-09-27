spring-boot
==================================================

# NAME

  spring-boot

# SYNOPSIS

  kubectl apply --recursive -f spring-boot

# SETTERS / SUBSTITUTIONS

kpt cfg list-setters spring-boot\ --include-subst
spring-boot/
      NAME          VALUE      SET BY         DESCRIPTION          COUNT   REQUIRED
  image-tag      1.14.2                 image tag                  1       No
  replicas       5                      need at least 5 replicas   1       No
  service-name   spring-boot            service name               8       No
--------------- -------------------- --------------
  SUBSTITUTION        PATTERN         REFERENCES
  image-value    nginx:${image-tag}   [image-tag]


# Description

kpt spring boot backage

# SEE ALSO

