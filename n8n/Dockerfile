FROM n8nio/n8n:latest

# Set environment variables
ENV N8N_HOST=logic.bdrllm.com
ENV N8N_PROTOCOL=https
ENV N8N_PORT=5678
ENV NODE_ENV=production
ENV N8N_ENCRYPTION_KEY=your-secret-key-here
ENV WEBHOOK_URL=https://logic.bdrllm.com/

# Optional: Install additional packages if needed
USER root
RUN apk add --update python3 py3-pip

# Switch back to node user (n8n default)
USER node

# The n8n data directory is already set as a volume in the base image
# VOLUME /home/node/.n8n

# The base image already exposes port 5678
# EXPOSE 5678

# The base image already has a CMD to run n8n